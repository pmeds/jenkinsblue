pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh 'npm version'
      }
    }

  }
  tools {
    nodejs 'njs'
  }
}