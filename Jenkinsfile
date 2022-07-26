pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''edgekv-importer --help

'''
        tool(name: 'njs', type: 'nodejs')
        sh 'npm version'
      }
    }

  }
}