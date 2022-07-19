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
            echo 'Test Step'
          }
        }

        stage('Test Par') {
          steps {
            echo 'Test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}