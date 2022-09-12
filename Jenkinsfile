pipeline {
    agent any

    options {
        buildDiscarder(logRotator(numToKeepStr: '5'))
    }

    stages {
        stage('SetUp') {
            steps {
                sh 'pip3 install -U pytest --user'
            }
        }
        stage('Test') {
            steps {
                sh 'python3 -m pytest aleko.py'
            }
        }
    }
}

