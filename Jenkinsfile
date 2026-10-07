pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/jayendrajadhav1991-oss/aaruapp.git'
            }
        }

        stage('Install') {
            steps {
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                bat 'npm test'
            }
        }

        stage('Build') {
            steps {
                bat 'npm run build'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
