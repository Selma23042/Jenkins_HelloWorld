pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/ton-utilisateur/ton-repo.git'
            }
        }
        stage('Compile') {
            steps {
                script {
                    sh 'javac HelloWorld.java'
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    sh 'java HelloWorld'
                }
            }
        }
    }
}
