pipeline {
  agent any

  stages {
    stage('Terraform automation') {
      steps {
        
        dir('terraform_resource/inst.tf') {
          
          sh 'terraform init'

          
          sh 'terraform plan -out=tfplan'

          
          sh 'terraform apply --auto-approve tfplan'
        }
      }
    }
  }
}

