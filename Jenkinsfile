pipeline {
  agent any
  stages {
    stage('install edgekv uploader') {
      environment {
        edgerc = 'edgerc'
      }
      steps {
        sh '''touch /var/lib/jenkins/.profile
wget https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh -P /var/lib/jenkins/
chmod 744 /var/lib/jenkins/install.sh
sh /var/lib/jenkins/install.sh'''
        sh '''cd /var/lib/jenkins/
pwd
mkdir ekvuploader
nvm install v14.20.0
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/index.js -P /var/lib/jenkins/ekvuploader
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/package-lock.json -P /var/lib/jenkins/ekvuploader
wget https://raw.githubusercontent.com/akamai/edgeworkers-examples/master/edgekv/utils/edgekv-importer/package.json -P /var/lib/jenkins/ekvuploader
cd /var/lib/jenkins/ekvuploader
node install -g


'''
      }
    }

  }
}