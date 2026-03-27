pipeline {
    agent any
    tools {
        jdk 'jdk-23' 
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/nissrine-elmniai/hello-world.git'
            }
        }

        stage('Compile HelloWorld') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run HelloWorld') {
            steps {
                bat 'java HelloWorld'
            }
        }

        stage('Compile Merci') {
            steps {
                bat 'javac Merci.java'
            }
        }

        stage('Run Merci') {
            steps {
                bat 'java Merci'
            }
        }

        stage('Compile DeRien') {
            steps {
                bat 'javac DeRien.java'
            }
        }

        stage('Run DeRien') {
            steps {
                bat 'java DeRien'
            }
        }
    }
}