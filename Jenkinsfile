pipeline {
  agent any
  stages {
    parameter()
    stage('error') {
      parallel {
        stage('error') {
          steps {
            echo 'hello'
          }
        }
        stage('stage2') {
          steps {
            echo 'a'
          }
        }
      }
    }
    stage('commit') {
      steps {
        echo 'commit'
      }
    }
  }
  environment {
    abc = '1'
    cde = 'true'
  }
}