pipeline {
    agent any
    stages {
        stage('Pull Code') {
            steps {
                echo 'Pulling from GitHub...'
                sh 'whoami'
                sh 'date'
                sh 'echo Build successful on AWS EC2!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying on EC2...'
                sh 'echo App is live!'
            }
        }
    }
}
