pipeline {
    agent { label 'nodejs' }
    stages {
        stage('install') {
            steps {
                sh 'npm install'
            }
        }
        stage('build') {
            steps {
                sh 'docker build . -t my-api:latest'
            }
        }
    }
}
