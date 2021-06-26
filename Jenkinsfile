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
                sh './vendor/bin/phpunit'
            }
        }
        stage('Deploy') {
            steps {
                sh '"cd ~/project/myblog; \
                git pull origin master; \
                composer install --optimize-autoloader --no-dev;
                php artisan migrate --force; \
                php artisan cache:clear; \
                php artisan config:cache "'
            }
        }
    }
}