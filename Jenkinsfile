pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/HarshG777/cpp-repo.git'
            }
        }
        stage('Build and Run') {
            steps {
                sh 'make all'
                sh 'make run'
            }
        }
    }
}
