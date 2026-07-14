
pipeline {
    agent any

    environment {
        REPO_URL = 'url'
        PROJECT_DIR = 'demo'
        APP_PORT = 'portnumber'
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Pulling code from GitHub ${REPO_URL}'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application'
            }
        }
    }
    post {
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
        always {
            echo 'Pipeline Completed.'
        }
    }
}

     
