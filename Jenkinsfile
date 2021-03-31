pipeline{
    stages{
        stage('Build'){
            docker build -t cbarraco/docker-android-sdk:latest .
        }
        stage('Deploy') {
            docker push cbarraco/docker-android-sdk:latest
        }
    }
}