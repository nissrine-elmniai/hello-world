pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/votre-utilisateur/votre-repo.git'
            }
        }

        stage('Compile HelloWorld') {
            steps {
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run HelloWorld') {
            steps {
                sh 'java HelloWorld'
            }
        }

        stage('Compile Merci') {
            steps {
                sh 'javac Merci.java'
            }
        }

        stage('Run Merci') {
            steps {
                sh 'java Merci'
            }
        }

        stage('Compile DeRien') {
            steps {
                sh 'javac DeRien.java'
            }
        }

        stage('Run DeRien') {
            steps {
                sh 'java DeRien'
            }
        }
    }
}