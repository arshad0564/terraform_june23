pipeline {
    agent any

    stages {
stage('Terraform Init') {
  steps {
    dir('/var/lib/jenkins/workspace/jenkins_terraform/tf_resource') {
      sh 'terraform init'
    }
  }
}

stage('Terraform Apply') {
  steps {
    dir('/var/lib/jenkins/workspace/jenkins_terraform/tf_resource') {
      sh 'terraform apply --auto-approve'
    }
  }
}

    }
}
