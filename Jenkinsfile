pipeline {
  agent any
  stages {
    stage('B0') {
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
            waitUntil() {
              sh 'a=1'
            }

          }
        }
        stage('b3') {
          steps {
            echo '333'
            script {
              ddddd
            }

          }
        }
      }
    }
  }
}