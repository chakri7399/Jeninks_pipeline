pipeline {
    agent{
        docker { image 'python:3.6-slim' }
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/chakri7399/Jeninks_pipeline.git']])
            }
        }
        stage('Test') {
            steps {
                sh 'python --version'
            }
        }
    }
}

