pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/Palash1214/Basic_of_UI_Template_File.git'
            }
        }

        stage('Build') {
            steps {
                echo "No build required for static website"
            }
        }

        stage('Test') {
            steps {
                echo "No tests defined"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying static files..."

                // Copy only required files
                sh 'cp index.html /var/www/html/'
                sh 'cp error.html /var/www/html/'
            }
    }
}
}
