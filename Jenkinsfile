pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/HexaEmbed/01_Automation.git'
            }
        }
        stage('Build') {
            steps {
                sh 'gcc -o app main.c'
            }
        }
        stage('Test') {
            steps {
                sh './app'
            }
        }
    }
}
