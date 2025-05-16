pipeline {
    agent any 

    stages {
        stage('CHECKOUT') {
            steps {
                echo "This is Checkout stage"
                checkout scmGit(branches: [[name: '*/main']], extensions: [], 
                userRemoteConfigs: [[credentialsId: 'ubuntu',
                url: 'https://github.com/Jenkins-hub121/Pipeline.git']])
            }
        }

        stage('BUILD') {
            steps {
                echo "This is Build stage"
            }
        }

        stage('TEST') {
            steps {
                echo "This is Test stage"
            }
        }

        stage('DEPLOY') {
            steps {
                echo "This is Deploy stage"
            }
        }
    }
}