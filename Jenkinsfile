pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'git@github.com:sadmanpieal/CICDwithJenkins-Assignment2.git'
            }
        }

        stage('Read and Print hello.txt') {
            steps {
                script {
                    def content = readFile('hello.txt')
                    echo "Contents of hello.txt:\n${content}"
                }
            }
        }
    }
}
