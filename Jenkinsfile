pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git --version
                git 'https://github.com/HarshG777/cpp-repo.git'
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
