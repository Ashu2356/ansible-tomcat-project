pipeline {
    agent any

    environment {
        JAVA_HOME = "/usr/lib/jvm/java-17-amazon-corretto.x86_64"
        PATH = "${JAVA_HOME}/bin:${env.PATH}"
    }

    stages {
        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook build_and_deploy.yml'
            }
        }
    }
}
