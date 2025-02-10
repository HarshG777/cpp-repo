pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                sh 'rm -rf cpp-refo || true'
                bat 'git branch: main, url: https://github.com/HarshG777/cpp-repo.git'
            }
        }
        stage('Build and Run') {
            steps {
                bat 'make all'
                bat 'make run'
            }
        }
    }
}
