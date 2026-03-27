pipeline {
    agent any
    
    tools {
        jdk 'JDK11'  
    }
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/nissrine-elmniai/hello-world.git'
            }
        }

        stage('Compile HelloWorld') {
            steps {
                bat 'javac HelloWorld.java'   // sh → bat
            }
        }

        stage('Run HelloWorld') {
            steps {
                bat 'java HelloWorld'         // sh → bat
            }
        }

        stage('Compile Merci') {
            steps {
                bat 'javac Merci.java'        // sh → bat
            }
        }

        stage('Run Merci') {
            steps {
                bat 'java Merci'              // sh → bat
            }
        }

        stage('Compile DeRien') {
            steps {
                bat 'javac DeRien.java'       // sh → bat
            }
        }

        stage('Run DeRien') {
            steps {
                bat 'java DeRien'             // sh → bat
            }
        }
    }
}