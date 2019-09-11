pipeline {
    agent { docker { image 'node:6.3' } }
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
