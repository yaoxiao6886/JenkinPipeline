pipeline {
  agent any
  stages {
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
}