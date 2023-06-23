pipeline {
  agent any

  stages {
    stage('Terraform automation') {
      steps {
          
          sh 'terraform init'

          
          sh 'terraform plan '

          
          sh 'terraform apply --auto-approve '
        }
      }
    }
  }
