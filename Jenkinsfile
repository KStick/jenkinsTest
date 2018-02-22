pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            sh 'echo "hello World i am stage 1"'
          }
        }
        stage('paralel') {
          steps {
            echo 'paralel'
          }
        }
        stage('mail') {
          steps {
            mail(subject: 'Test', body: 'This is an automated test mail', from: 'super-stick@hotmail.com', to: 'super-stick@hotmail.com')
          }
        }
      }
    }
    stage('end') {
      steps {
        echo 'Done'
      }
    }
  }
}