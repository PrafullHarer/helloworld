
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out project...'
                checkout scm
            }
        }

        stage('Python Version') {
            steps {
                bat 'python --version'
            }
        }

        stage('Run Python Program') {
            steps {
                echo 'Running Hello World Program...'
                bat 'python hello_world.py'
            }
        }

        stage('Build Success') {
            steps {
                echo 'Hello World project executed successfully!'
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
