pipeline {
    agent any

    stages {
        stage('Run Ansible Playbook') {
  steps {
    sh "ansible-playbook build_and_deploy.yml"
  }
}
    }
}
