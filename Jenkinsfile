//declarative pipeline
pipeline{
  agent any  
  stages {
    stage('1.CodeClone'){
      steps{
          https://github.com/autoking777/JenkinsPipelineDemo.git
      }
    } 
    stage('2.mavenBuild'){
      steps{
      sh "mvn clean package"
      } 
    }
    stage('3.CodeQuality') {
      steps{
      sh "echo reports done"
      //sh "mvn sonar:sonar"
      } 
    }
    stage('4.uploadToNexus'){
      steps{
      sh "echo artifacts uploaded"
      //sh "mvn deploy"
      } 
    }
   } 
  }
