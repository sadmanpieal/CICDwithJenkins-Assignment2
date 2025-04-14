pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', credentialsId: '52ef2c19-c6fc-4b0e-b0d2-19ea9ef834be', url: 'git@github.com:sadmanpieal/CICDwithJenkins-Assignment2.git'
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
