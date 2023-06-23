pipeline {
    agent any

    stages {
stage('Terraform Init') {
  steps {
    sh 'terraform init -chdir=/var/lib/jenkins/workspace/jenkins_terraform'
  }
}

stage('Terraform Apply') {
  steps {
    sh 'terraform apply -auto-approve -chdir=/var/lib/jenkins/workspace/jenkins_terraform'
  }
}
    }
}
