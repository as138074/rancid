pipeline {

    agent any

    stages {
        stage('Preparation') {
            steps {
                sh 'whoami'
                sh 'sudo apt install -y automake cvs expect iputils-ping perl po-debconf telnet openssh-client build-essential'
            }
        }
        stage('Build') {
            steps {
                sh './configure'
                sh 'make'
            }
        }
    }
}
