pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building ...'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing Firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}