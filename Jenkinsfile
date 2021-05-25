pipeline {
  agent {
    docker {
      image 'molecule_local/milcom/centos7-systemd'
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