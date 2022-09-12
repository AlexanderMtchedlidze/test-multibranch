pipeline {
    agent any

    options {
        buildDiscarder(logRotator(numToKeepStr: '5'))
    }

    stages {
        stage('Hello') {
            steps {
                sh 'python3 --version'
                sh 'pip3 install -U pytest --user'
                sh 'pip3 pytest --version'
                echo 'Hello World'
            }
        }
    }
}

