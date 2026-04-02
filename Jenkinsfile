pipeline {
    agent any
    stages {
        stage('Pull Code') {
            steps {
                echo 'Pulling from GitHub... lets see it is working or not '
                sh 'whoami'
                sh 'date'
                sh 'echo Build successful on AWS EC2!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying on EC2...'
                sh 'echo App is live!'
                echo ' So if  i seing this built in the jenkins that means the web-hook is worked '
                echo 'hi babe'
            }
        }
    }
}
