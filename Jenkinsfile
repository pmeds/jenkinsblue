pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''./home/jenkins/install.sh
nvm install v14.20.0'''
      }
    }

  }
}