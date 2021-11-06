pipeline {
    agent none
    stages {
        stage('Fetch git repo and build docker image') {
            agent { label 'docker-agent-1' }
            steps {
                git scm
                sh 'docker build -t myImage .'
                sh 'docker images'
            }
        }
    }
}