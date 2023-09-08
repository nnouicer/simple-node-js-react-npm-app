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
      }
    }

    stage('build') {
      steps {
        sh 'npm run build'
      }
    }

    stage('Deploy') {
      steps {
        sh '''npm run deploy
'''
      }
    }

  }
}