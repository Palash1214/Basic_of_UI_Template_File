pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Jenkins automatically checks out code
                echo 'Code fetched from GitHub'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building app..."'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                mkdir -p /var/www/html
                cp index.html /var/www/html/
                '''
            }
        }
    }
}
