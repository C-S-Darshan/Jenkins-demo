pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'No build needed for Python script, just a demo'
            }
        }

        stage('Test') {
            steps {
                echo 'Running unit tests'
                bat 'python -m unittest test_app.py'
                echo 'Unit tests completed'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished'
        }
    }
}
