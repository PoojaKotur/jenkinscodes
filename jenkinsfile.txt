pipeline {
    agent any

    stages {
        stage('Code pull') {
            steps {
                echo 'Hi Jenkins I am pulling code from Github'
            }
        } 
        stage('Build') {
            steps {
                echo 'I am building one docker image with the help of Naren'
            }
        }
        stage('deploy') {
            steps {
                echo 'Running container from above built docker image and deploy NodeJS on it'
            }
        } 
    }
}
