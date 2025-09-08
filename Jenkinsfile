pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    credentialsId: 'your-github-cred-id',
                    url: 'https://github.com/yourusername/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Example: npm install or maven build
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example: npm test or pytest
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to server...'
                // Example: copy files to a web server or run ansible/ssh commands
            }
        }
    }
}
