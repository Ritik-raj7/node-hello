pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/your-user/your-node-repo.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run App') {
            steps {
                sh 'npm start &'
                sh 'echo "App is running"'
            }
        }
    }
}
