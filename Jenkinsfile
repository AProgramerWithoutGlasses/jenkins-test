pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    docker.image('golang:1.24').inside('-w /app') { // 指定Linux路径 /app 作为工作目录
                        sh 'go version'
                        sh 'go build -o myapp'
                    }
                }
            }
        }
    }
}