pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Pulls latest code from GitHub
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Example: copy files to server or build docker
                sh 'echo App Deployed Successfully'
            }
        }
    }
}
