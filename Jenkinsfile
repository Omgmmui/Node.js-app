pipeline {
  agent any

  tools {
    nodejs 'nodejs'
  }

  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', url: 'https://github.com/Omgmmui/Node.js-app.git'
      }
    }

    stage('Install Dependencies') {
      steps {
        bat 'npm install'
      }
    }

    stage('Run App') {
      steps {
        bat 'node app.js'
      }
    }
  }
}
