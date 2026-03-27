pipeline {
    agent any
    
    tools {
        // Le nom ici doit être EXACTEMENT le même que celui 
        // configuré dans "Global Tool Configuration"
        jdk 'jdk-23' 
    }
    
    stages {
        stage('Compilation') {
            steps {
                // Sous Windows, on utilise 'bat'
                bat 'javac HelloWorld.java'
                bat 'java HelloWorld'
            }
        }
    }
}