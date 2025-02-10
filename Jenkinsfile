pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git ''
            }
        }
        stage('Build') {
            steps {
                sh 'g++ -o hello hello.cpp'
            }
        }
        stage('Run') {
            steps {
                sh './hello'
            }
        }
    }
}
