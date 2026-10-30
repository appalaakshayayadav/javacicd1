pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }

    post {
        success {
            echo 'Java CI/CD Pipeline Completed Successfully!'
        }
        failure {
            echo 'Java CI/CD Pipeline Failed!'
        }
    }
}