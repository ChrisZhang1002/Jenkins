pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/ChrisZhang1002/Jenkins', branch: 'test1')
      }
    }

    stage('bash') {
      parallel {
        stage('bash') {
          steps {
            sh '''ls -la
pwd'''
          }
        }

        stage('bash2') {
          steps {
            sh '''cont="hello world!"
echo ${cont}'''
          }
        }

        stage('docker run busybox') {
          steps {
            sh 'docker run busybox'
          }
        }

      }
    }

  }
}