pipeline {
    agent {label 'docker'}
    stages {
        stage('docker') {
            steps {
                sh """curl -fsSL https://get.docker.com -o get-docker.sh
                      sh get-docker.sh
                      sudo usermod -aG docker ubuntu
                      exit
                      ssh ubuntu@3.80.125.147
                      docker info
                   """
            }
        }
    }
}