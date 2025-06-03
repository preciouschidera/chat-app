pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/preciouschidera/chat-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Start App') {
            steps {
                sh 'nohup node app.js &'
            }
        }
    }
}

