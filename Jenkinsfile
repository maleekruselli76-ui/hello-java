pipeline {
    agent any
    environment {
        PATH = "C:\\Program Files\\Docker\\Docker\\resources;${env.PATH}"
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
        stage('Docker Build') {
            steps {
                bat '"C:/Users/malee/AppData/Local/Programs/DockerDesktop/resources/bin/docker.exe" build -t my-app .'
            }
        }
    }
}
