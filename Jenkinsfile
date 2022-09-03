pipeline {
  agent {
    docker {
      image 'python:2-alpine' 
    }
  }
  stages {
    stage('Build') {
      steps {
        sh '''python time.py'''
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