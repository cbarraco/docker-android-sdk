pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''docker build -t cbarraco/docker-android-sdk:latest .
'''
      }
    }

    stage('Deploy') {
      steps {
        sh 'docker push cbarraco/docker-android-sdk:latest'
      }
    }

  }
}