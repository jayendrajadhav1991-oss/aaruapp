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
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
