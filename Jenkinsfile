pipeline {
    agent any    
    tools {
        terraform 'Terraform'
    }
    stages{
        stage('Clone Repo'){
            steps{
                sh 'https://github.com/rameshsampathi/terraformsingleinstance.git'
            }
        }
        stage('terraform init'){
            steps{
                sh 'terraform init'
            }
        }
        stage('terraform plan'){
            steps{
                sh 'terraform plan'
            }
        }
        stage('terraform apply'){
            steps{
                sh 'terraform apply  --auto-approve' 
            }
        } 
    }
}                       