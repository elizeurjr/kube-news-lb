pipeline {
    agent any

    stages {

        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("elizeurjr/kubenews:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }
}