pipeline {
  agent {
    docker {
      image 'Centos'
    }

  }
  stages {
    stage('syntax') {
      steps {
        sh '''cd $ROLEDIR
molecule syntax'''
      }
    }

  }
  environment {
    ROLEDIR = 'ansible/roles/webserver'
  }
}