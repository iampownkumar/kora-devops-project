pipeline{
    agent any {
          stages {
                stage('pull the code from the git hub') {
                    steps{ 
                             echo 'Pulling the repo from the github '
                              sh 'whoami'
                              sh 'date'
                              echo 'Pulling Succesfull from the github via Amazon EC2 '
                                }
                    stage('Deploy') { 
                                      steps{
                                        echo 'Project successfully deployed in the amazon EC2 service '
                                        sh 'echo app is live '
                                      }
                                          }

  
                }
        }
    }
}
