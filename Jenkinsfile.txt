pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checkout stage'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage'
            }
        }

        stage('Docker Build') {
            steps {
                echo 'Docker build stage'
            }
        }
    }
}
