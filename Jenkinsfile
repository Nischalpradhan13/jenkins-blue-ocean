pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''date
pwd'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'This is test stage'
          }
        }

        stage('Second test') {
          steps {
            echo 'second test print'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy the job'
      }
    }

  }
}