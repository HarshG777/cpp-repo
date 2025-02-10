pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git '<repository-url>'
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
