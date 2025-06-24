pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/Ritik-raj7/node-hello.git'
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
