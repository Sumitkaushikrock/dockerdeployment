pipeline {
    agent none
    stages {
        stage('Fetch git repo and build docker image') {
            agent { label 'docker-agent' }
            steps {
/*                git credentialsId: 'first-repo', url: 'http://172.16.238.2:3000/git-user/first-repo.git'
                sh 'docker build -t hello_py:1 .'*/
                sh 'docker images'
            }
        }
    }
}