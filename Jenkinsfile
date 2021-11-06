pipeline {
    agent none
    stages {
        stage('Fetch git repo and build docker image') {
            agent { label 'docker-agent-1' }
            steps {
                sh 'git clone https://github.com/Sumitkaushikrock/dockerdeployment'
                sh 'docker -H tcp://docker.for.mac.localhost:3375 build -t sumitkaushik445/dockerdeployment .'
                sh 'docker -H tcp://docker.for.mac.localhost:3375 images'
            }
        }
    }
}