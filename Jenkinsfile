pipeline {
    agent any

    environment {
        JAVA_HOME = "/path/to/java"   // update this path to your actual JAVA_HOME
        MAVEN_HOME = "/path/to/apache-maven-3.9.11"  // update to your Maven path
        PATH = "${env.JAVA_HOME}/bin:${env.MAVEN_HOME}/bin:${env.PATH}"
    }

    stages {
        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook build_and_deploy.yml'
            }
        }
    }
}
