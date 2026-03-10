pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Setujha90/DevOps.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building Project...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Project...'
            }
        }
        stage('Deploy') {
            steps {
                    bat '''
                if not exist C:\\deploy-demo mkdir C:\\deploy-demo
                copy index.html C:\\deploy-demo
                '''
            }
        }
    }
}