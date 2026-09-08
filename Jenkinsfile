pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building the Java application...'
                bat 'javac HelloJenkins.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the Java application...'
                bat 'java HelloJenkins'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                echo 'Deployment completed successfully.'
            }
        }
    }

    post {
        success {
            echo 'CI/CD Pipeline completed successfully!'
        }
        failure {
            echo 'CI/CD Pipeline failed.'
        }
    }
}