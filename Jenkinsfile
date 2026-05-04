pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo 'Cloning repository...'
                git 'https://github.com/abhijeetshirke61/Tour-Management-System.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing project...'
            }
        }

        stage('Deploy to XAMPP') {
            steps {
                echo 'Deploying to XAMPP htdocs...'

                bat '''
                xcopy /E /I /Y * C:\\xampp\\htdocs\\tour
                '''
            }
        }

    }
}
