pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                echo 'checking out from git'
                git branch: 'main', url: 'https://github.com/Francis-88-cpu/javamoney-shelter.git'
            }
        }

        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('package') {
            steps {
                sh 'mvn package'
            }
        }

        stage('docker build') {
            steps {
                sh 'docker'
            }
        }
        
    }
}