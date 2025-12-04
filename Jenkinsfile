pipeline {
    agent any

    stages {
        stage('Trigger Ansible CI/CD Pipeline') {
            steps {
                sh '''
                ssh -o StrictHostKeyChecking=no ubuntu@18.116.65.231 \ 
                "cd project-ansible && ansible-playbook -i inventory.ini site.yml"
                '''
            }
        }
    }
}
