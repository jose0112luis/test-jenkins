pipeline {
  agent any
  tools {
    nodejs 'node-18.12.1'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
    stage('Run Test') {
      steps {
        sh 'npm test'
      }
    }
  }
}