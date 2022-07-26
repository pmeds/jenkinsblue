pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        EDGERC = credentials('pauledgerc')
      }
      steps {
        sh '''edgekv-importer --help
akamai --edgerc ${EDGERC} edgeworkers --accountkey 1-6JHGX status 50596'''
      }
    }

  }
  tools {
    nodejs 'njs'
  }
}
