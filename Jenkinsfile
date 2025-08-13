pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'python3 --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'python3 src/main.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application (simulation)...'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
