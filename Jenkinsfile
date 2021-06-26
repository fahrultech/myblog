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
                echo 'Testing..Mbas'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....again'
            }
        }
    }
}