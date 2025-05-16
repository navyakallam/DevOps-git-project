pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning the GitHub repository...'
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Building Docker image...'
                sh 'docker build -t devops-git-project .'
            }
        }

        stage('Run Container') {
            steps {
                echo 'Running Docker container...'
                sh 'docker run -d -p 8080:80 --name devops-git-container devops-git-project'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the logs.'
        }
    }
}


