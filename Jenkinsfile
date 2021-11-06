pipeline {
    agent none
    stages {
        stage('Fetch git repo and build docker image') {
            agent { label 'docker-agent-1' }
            steps {
                sh 'git clone https://github.com/Sumitkaushikrock/dockerdeployment'
                sh 'docker build -t myImage .'
                sh 'docker images'
            }
        }
    }
}