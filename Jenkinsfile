
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install pytest') {
            steps {
                sh 'python3 -m pip install pytest'
            }
        }

        stage('Run Unit Tests') {
            steps {
                sh 'python3 -m pytest -v'
            }
        }
    }
}
