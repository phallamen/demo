pipeline{
  agent any;
  tools {
        maven 'maven'
    }
  stages{
    stage("Code Review"){
      steps{
          echo "Code reviewing, hold on!"
          withSonarQubeEnv('sonarqube'){
            sh "sonar-scanner " 
             
          }
      }
    }
    stage("Building App"){
      steps{
        sh 'mvn clean package'
        
      }
    }
  }
}
