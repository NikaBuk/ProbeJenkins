pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'python:2-alpine' 
        }
      }
    
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