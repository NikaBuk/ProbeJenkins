pipeline {
  agent { docker { image 'python:3.10.1-alpine' } }
  stages {
    stage('Build') {
      steps {
        sh 'python --version'
        sh 'python time.py'
      }
    }

    stage('Test') {
      steps {
        sh 'echo \'Testing...\''
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo \'Deploying...\''
      }
    }

  }
}