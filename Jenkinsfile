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
                echo 'Hello World'
            }
        }
    }
}

