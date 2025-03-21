pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/lavanya.m/https://github.com/lavanyamadarasu-cloudside/test-repository.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t hello-world-image .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run --rm hello-world-image'
                }
            }
        }
    }
}
