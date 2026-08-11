pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                dir('src') {
                    // Compile hi.java
                    sh 'javac hi.java'
                }
            }
        }
        stage('Run') {
            steps {
                dir('src') {
                    // Run the hi class
                    sh 'java hi'
                }
            }
        }
    }
}
