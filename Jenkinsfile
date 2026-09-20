pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/HexaEmbed/01_Automation.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'pip3 install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                sh 'pytest tests/'
            }
        }
    }
}
