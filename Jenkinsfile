pipeline {
    agent any 
    stages {
        stage('Cloudformation template') { 
            steps {
            sh "aws cloudformation create-stack --stack-name vpc --template-body file://file1 --region 'us-east-1'"     
             }
         }
     }
  }

