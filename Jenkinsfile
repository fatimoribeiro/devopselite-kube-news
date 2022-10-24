pipeline {
    agent any

    stages {
        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = Docker.Build("fatimoribeiro/devopselite-kube-news:${env_BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}