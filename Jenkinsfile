pipeline {
    agent any

    stages {
        stage('Run CI/CD using Ansible') {
            steps {
                sh 'ansible-playbook -i inventory.ini site.yml'
            }
        }
    }
}
