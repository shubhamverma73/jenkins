pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        powershell 'echo "Programming Path"'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'How are you Developer?'
          }
        }

        stage('Test Stage') {
          steps {
            echo 'This is stage Message under Test'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Now we are on Deploy stage'
        sleep 10
      }
    }

  }
}