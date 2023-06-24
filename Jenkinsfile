pipeline {
    agent any

    stages {
stage('Terraform Init') {
  steps {
    dir('tf_resource') {
      sh 'terraform init'
    }
  }
}

stage('Terraform Apply') {
  steps {
    dir('tf_resource') {
      sh 'terraform apply --auto-approve'
    }
  }
}

    }
}
