pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3001:3001'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm config set proxy=http://10.178.148.69:3128'
        sh 'npm config set https-proxy=http://10.178.148.69:3128'
        sh 'npm install'
      }
    }

  }
}
