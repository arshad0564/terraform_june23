pipeline {
    agent any

    stages {
        stage('Terraform init') {
            steps {

                 sh 'terraform init /var/lib/jenkins/workspace/jenkins_terraform'
        }
        }
        stage('Terraform apply') {
            steps {

                sh 'terraform apply --auto-approve /var/lib/jenkins/workspace/jenkins_terraform'
            }
                    
            }
    }
}
