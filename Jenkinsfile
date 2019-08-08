pipeline {
    agent any

    stages {
        stage('CLoudformation Deployment') {
            steps {
                echo 'Cloudfromation Started'
              sh ' ansible-playbook deploy.yml '  
            }
        }
