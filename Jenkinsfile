pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'composer install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..Bro Mas'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....Mas'
            }
        }
    }
}