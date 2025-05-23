pipeline{
    agent any
        stages{
            stage('checkout code'){
                steps{
                    echo " this is my first pipeline job"
                    checkout scmGit(branches:
                     [[name: '*/main']], extensions: [], 
                     userRemoteConfigs: [[credentialsId: 'git', 
                     url: 'https://github.com/Jenkins-hub121/Pipeline.git']])
                }
            }
            stage('build') {
                steps{
                    echo "this is my 2nd pipeline job"
                }
            }
            stage('any_name'){
                steps{
                    echo "this is my 3rd pipeline job"
                }
            }
        }
    }