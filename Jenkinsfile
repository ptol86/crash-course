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
                echo "Zaebalooooooo"
                bat "docker-compose -f ./docker-compose.yml up --build -d"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}