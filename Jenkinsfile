pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'docker build -t .https://hub.docker.com/repositories/thulasi0512'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    sh 'docker push 'https://hub.docker.com/repositories/thulasi0512
                }
            }
        }
    }
    triggers {
        pollSCM('')
    }
