pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/Omgmmui/Node.js-app.git'
      }
    }

    stage('Install Dependencies') {
      steps {
        bat 'npm install'
      }
    }

    stage('Run App Test') {
      steps {
        bat 'node app.js'
      }
    }
  }
}
