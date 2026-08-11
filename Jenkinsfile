pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                bat 'javac hi.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java hi'
            }
        }
    }
    post {
        success { echo 'BUILD SUCCESSFUL' }
        failure { echo 'BUILD FAILED' }
    }
}
