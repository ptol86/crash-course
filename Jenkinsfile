pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo "build started"
                bat "docker-compose -f ./docker-compose.yml up --build -d"
                echo "build finished"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }
}