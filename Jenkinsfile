pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''cd /home/jenkins_home
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/index.js
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/package-lock.json
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/package.json
npm install -g
'''
      }
    }

  }
}