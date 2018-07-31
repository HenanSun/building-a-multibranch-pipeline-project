pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello world!"'
        sh '''if (params.ACTION == \'apply\') {
				            sh \'kubectl apply -f ./tmp-gitclone/apply.yaml\'
				        } else {
				            sh \'kubectl set image deployment/${AppName} *=${ImageName}\'
				        }'''
        }
      }
    }
  }