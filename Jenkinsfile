pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                bat 'javac sample.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java sample'
            }
        }
    }

    post {
        success {
            echo 'BUILD SUCCESSFUL'
        }
        failure {
            echo 'BUILD FAILED'
        }
    }
}