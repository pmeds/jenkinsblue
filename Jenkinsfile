pipeline {
  agent any
  tools {nodejs "njs"}
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''edgekv-importer --help

'''
        sh 'npm version'
      }
    }

  }
}
