pipeline {
    agent any
     environment {
        AWS_ACCESS_KEY_ID = credentials('AKIAXNHDNEQCP3UWKVS3')
        AWS_SECRET_ACCESS_KEY = credentials('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')
     }
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
