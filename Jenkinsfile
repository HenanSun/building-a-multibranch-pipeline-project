pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          agent any
          steps {
            sh 'echo "Hello world!"'
            echo 'sss'
          }
        }
        stage('b2') {
          steps {
            echo 'ddd'
          }
        }
        stage('b3') {
          steps {
            echo '333'
          }
        }
      }
    }
  }
}