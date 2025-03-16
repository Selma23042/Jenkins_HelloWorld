pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/selma23042/Jenkins_HelloWorld.git'
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

