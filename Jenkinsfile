pipeline{
  agent any;
  tools {
        maven 'maven'
    }
  stages{
    stage("Building App"){
      steps{
        sh 'mvn clean package'
        
      }
    }
    stage("Code Review"){
      steps{
          echo "Code reviewing, hold on!"
          withSonarQubeEnv('sonarqube'){
            sh "sonar-scanner " 
             
          }
      }
    }
  }
}
