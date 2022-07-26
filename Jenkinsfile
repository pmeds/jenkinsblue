pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''cd /home/jenkins
nvm install v14.20.0'''
      }
    }

  }
}