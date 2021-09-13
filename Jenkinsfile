pipeline{
  agent any;
  tools {
        maven 'apache-maven-3.0.1' 
    }
  stages{
    stage("Code Review"){
      steps{
          echo "Code reviewing, hold on!"
      }
    }
    stage("Building App"){
      steps{
        sh 'mvn --version'
      }
    }
  }
}
