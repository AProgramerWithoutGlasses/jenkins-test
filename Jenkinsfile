pipeline {
    agent { docker 'golang:1.24' } // 使用Go 1.22的官方Docker镜像
    stages {
        stage('Build') {
            steps {
                sh 'go version' // 检查Go版本
                sh 'go build -o myapp' // 编译Go程序，假设你的主文件是main.go
            }
        }
    }
}
