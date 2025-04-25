pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/your-username/your-repo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-app:latest .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run -d -p 8080:80 --name my-container my-app:latest'
            }
        }
    }
}
