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
      }
    }
    stage('end') {
      steps {
        echo 'Done'
      }
    }
  }
}