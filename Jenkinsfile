pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh 'npm version'
        sh '''wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/index.js 
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/package-lock.json 
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/package.json 
npm install -g'''
      }
    }

  }
  tools {
    nodejs 'njs'
  }
}