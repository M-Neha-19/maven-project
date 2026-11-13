pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/M-Neha-19/maven-project.git'
            }
        }

        stage('Compile') {
            steps {
                bat '''set "PATH=https://github.com/M-Neha-19/maven-project.git" mvn compile'''
            }
        }

        stage('Test') {
            steps {
                bat '''set "PATH=https://github.com/M-Neha-19/maven-project.git" mvn test'''
            }
        }

        stage('Package') {
            steps {
                bat '''set "PATH=https://github.com/M-Neha-19/maven-project.git" mvn package'''
            }
        }
    }
}