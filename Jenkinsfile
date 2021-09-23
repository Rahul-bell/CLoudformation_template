pipeline {
    agent any 
    lable 'master'
    environment {
        AWS_ACCESS_KEY_ID     = credentials('jenkins-aws-secret-key-id')
        AWS_SECRET_ACCESS_KEY = credentials('jenkins-aws-secret-access-key')
    stages {
        stage('Cloudformation template') { 
            steps {
            sh "aws cloudformation create-stack --stack-name vpc --template-body file://file1 --region 'us-east-1'"     
             }
         }
     }
  }
}
