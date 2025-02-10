pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
                git 'https://github.com/HarshG777/cpp-repo.git'
                sh 'ls -l'  // Verify that hello.cpp exists
            }
        }
        stage('Build') {
            steps {
                echo 'Building C++ program...'
                sh 'g++ -v -o hello hello.cpp || exit 1'  // Verbose build output
            }
        }
        stage('Run') {
            steps {
                echo 'Running C++ program...'
                sh './hello'
            }
        }
    }
}
