pipeline {
  agent any

  stages {
    stage('Terraform automation') {
      steps {
        
        dir('jenkins_terraform/terraform_resource/inst.tf') {
          
          sh 'terraform init'

          
          sh 'terraform plan '

          
          sh 'terraform apply --auto-approve '
        }
      }
    }
  }
}
