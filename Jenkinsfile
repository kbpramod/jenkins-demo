pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/kbpramod/jenkins-demo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build successful!"'
            }
        }
    }
}
