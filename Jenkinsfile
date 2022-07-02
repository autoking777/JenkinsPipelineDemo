pipeline{
  agent any 
  tools{
    maven "maven3.8.5"
  }
  stages{
    stage('1.clone'){
      steps{
            sh "echo clonning the latest version of the code" 
            https://github.com/autoking777/JenkinsPipelineDemo.git
            sh "echo clonning successful"
      }
    }  
      stage('2.Build'){
       steps{
        sh "echo validation, compilation, testing and package"
        sh "echo testing successful and ready to package"
        sh "mvn clean package"
      }
      }
  }
}
