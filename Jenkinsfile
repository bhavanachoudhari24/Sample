
pipeline{
    agent any
    parameters {
        choice(name: 'ENV', choices: ['dev', 'qa', 'prod'], description: 'Select environment')
    }
    stages{
        stage("checkout"){
            steps{
            echo "code checkout"
            checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'bhavanachoudhari24', url: 'https://github.com/bhavanachoudhari24/Sample.git']])
            echo "code checkout successful-11"
        }}
        stage ("build"){
            steps{
              echo "code build"
        }}
        stage("upload to docker hub1"){
            steps{
              echo "image upload"
        }}
        stage("deploy"){
            steps{
              echo "code deploy"
        }}
     }
    }
    
    
    
    
