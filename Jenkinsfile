pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''edgekv-importer --help
akamai install edgeworkers'''
      }
    }

  }
  tools {
    nodejs 'njs'
  }
}