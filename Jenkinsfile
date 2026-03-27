pipeline {
    agent any
    stages {
        stage('Hello World') {
            steps {
                // Compilation et exécution de HelloWorld
                bat 'javac HelloWorld.java'
                bat 'java HelloWorld'
            }
        }
        stage('Merci') {
            steps {
                // Compilation et exécution de Merci
                bat 'javac Merci.java'
                bat 'java Merci'
            }
        }
        stage('DeRien') {
            steps {
                // Compilation et exécution de DeRien
                bat 'javac DeRien.java'
                bat 'java DeRien'
            }
        }
    }
}