pipeline {
    agent any    
    tools {
        terraform 'Terraform'
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
        stage('terraform destroy'){
            steps{
                sh 'terraform destroy  --auto-approve' 
                sleep 20
        }
    } 
}    
    
    
    
    
