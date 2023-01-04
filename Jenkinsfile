pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/ChrisZhang1002/Jenkins', branch: 'test1')
      }
    }

    stage('bash') {
      steps {
        sh 'ls -la'
      }
    }

  }
}