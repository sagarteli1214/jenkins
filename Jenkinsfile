pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'TestStep'
          }
        }

        stage('Test Par') {
          steps {
            echo 'Test Par'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
        sleep 13
      }
    }

  }
}