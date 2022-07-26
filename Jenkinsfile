pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''wget https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh /var/lib/jenkins/
chmod 744 /var/lib/jenkins/install.sh
sh /var/lib/jenkins/install.sh'''
      }
    }

  }
}