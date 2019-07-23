pipeline {
  agent any
  parameters{
      choice(
         name: 'door_choice',
         choices: 'one\ntwo\nthree\nfour\nfive\nsix',
         description: 'door'            
      )
  }
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
  environment {
    abc = '1'
    cde = 'true'
  }
}