pipeline {
    agent any

    tools {
        maven 'maven 3.9.12'
    }
    
    environment {
        DOCKER_IMAGE = "demo-app"
        CONTAINER_NAME = "springboot-container"
        JAR_FILE_NAME = "app.jar"
        PORT = "8081"

        REMOTE_USER = "ec2-user"
        REMOTE_HOST = "3.35.212.107"
        REMOTE_DIR = "/home/ec2-user/deploy"
        SSH_CREDENTIALS_ID = "f534a5fe-c36d-45a6-ae20-f1fee5634f61"
    }

    stages {
        stage('Git Checkout'){
            steps {
                 checkout scm
            }
        }
    }
}