
pipeline{
    agent any
    stages{
        stage("checkout"){
            steps{
            echo "code checkout"
            checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'bhavanachoudhari24', url: 'https://github.com/bhavanachoudhari24/Sample.git']])
            echo "code checkout successful-1"
        }}
        stage ("build"){
            steps{
              echo "code build"
        }}
        stage("upload to docker hub"){
            steps{
              echo "image upload"
        }}
        stage("deploy"){
            steps{
              echo "code deploy"
        }}
     }
    }
    
    
    
    
