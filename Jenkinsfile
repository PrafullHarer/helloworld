
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Project checkout successful'
            }
        }

        stage('Python Version') {
            steps {
                bat '"C:\Users\student\AppData\Local\Programs\Python\Python311\python.exe" --version'
            }
        }

        stage('Run Python Program') {
            steps {
                bat '"C:\Users\student\AppData\Local\Programs\Python\Python311\python.exe" hello_world.py'
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
