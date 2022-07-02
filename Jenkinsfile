//declarative pipeline
pipeline{
  agent any  
  tools {
    maven "maven3.8.4"
  }
  triggers {
  pollSCM '* * * * * '
}
  stages {
    stage('1.CodeClone'){
      steps{
          git branch: 'stage', credentialsId: 'GitHubCredentials', url: 'https://github.com/LandmakTechnology/web-app'
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
