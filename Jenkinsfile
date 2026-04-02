pipeline {
    agent any
    stages {
        stage('Pull Code') {
            steps {
                echo 'Code pulled from GitHub'
                sh 'ls -la'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t kora-web:latest .'
                sh 'docker images | grep kora-web'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker stop kora-web || true'
                sh 'docker rm kora-web || true'
                sh 'docker run -d --name kora-web -p 3000:80 kora-web:latest'
                sh 'echo App deployed at port 3000'
            }
        }
    }
}