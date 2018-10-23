pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Build') {
            steps {
                sh 'python --version'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploy"'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Test"'
            }
        }

        stage('Release') {
            steps {
                sh 'echo "Release"'
            }
        }

        stage('Deploy to Prod') {
            steps {
                input message: 'Are you sure you want to deploy to Prod? (Click "Proceed" to continue)'
                sh 'echo "Deploy to Prod"'
            }
        }
    }
}
