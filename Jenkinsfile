
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/kanishka9875/Jenkins-Demo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Java program...'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Java program...'
                bat 'java HelloWorld'
            }
        }
    }
}
