pipeline {
    agent any

    stages {

        stage('Clone Repo') {
            steps {
                git 'https://github.com/umaanilyatham/jenkins-repo.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                bat 'ansible-playbook -i inventory deploy.yml'
            }
        }

    }
}