
pipeline{
    agent any
    stages{
        stage("checkout"){
        steps {
            withCredentials([string(credentialsId: 'jenkinsPAT', variable: 'jenkinsPAT')]) {
                sh 'echo $TOKEN'
            }
}
        stage("checkout"){
            steps{
            echo "code checkout"
            git url:"https://github.com/bhavanachoudhari24/Sample.git", branch:"main"
            echo "code checkout successful-first"
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
    
    
    
    
