pipeline {
  agent any

  stages {
    stage('Terraform automation') {
      steps {
        
        dir('jenkins_terraform/terraform_resource/init.tf') {
          
          sh 'terraform init'

          
          sh 'terraform plan -out=tfplan'

          
          sh 'terraform apply --auto-approve tfplan'
        }
      }
    }
  }
}

