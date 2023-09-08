pipeline {
  agent {
    docker {
      image 'node:18.17.1-alpine3.18'
    }

  }
  stages {
    stage('welcome') {
      steps {
        sh 'echo "coucou"'
      }
    }

    stage('installer') {
      steps {
        sh '''npm install
'''
        sh 'npm run build'
      }
    }

  }
}