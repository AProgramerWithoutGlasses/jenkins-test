pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'docker run --rm -v "%CD%:/app" -w /app golang:1.24 go version'
                bat 'docker run --rm -v "%CD%:/app" -w /app golang:1.24 go build -o myapp'
            }
        }
    }
}