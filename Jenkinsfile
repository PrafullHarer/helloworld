
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Project checkout successful'
            }
        }

        stage('Check Python') {
            steps {
                bat 'python --version'
            }
        }

        stage('Run Hello World') {
            steps {
                bat 'python hello_world.py'
            }
        }

    }

    post {
        success {
            echo 'BUILD SUCCESSFUL!'
        }

        failure {
            echo 'BUILD FAILED!'
        }
    }
}
