pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'I want to develop the code'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'I want to build the code'
          }
        }

        stage('Test') {
          steps {
            echo 'I want to test the code'
          }
        }

        stage('Deploy') {
          steps {
            echo 'I want to deploy the code'
          }
        }

      }
    }

  }
}