pipeline{
  agent any;
  tools {
        maven 'maven' 
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
