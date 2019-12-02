pipeline {
  agent {
    docker {
      image 'python_msg_clean:'
      args '-p 3001:3001'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

  }
}
