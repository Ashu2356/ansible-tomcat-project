pipeline {
    agent any

    stages {
        stage('Run Ansible Playbook') {
            steps {
                sh '''
                    ansible-playbook -i inventory/build_and_deploy.yml
                '''
            }
        }
    }
}
