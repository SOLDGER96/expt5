pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from repository
                git branch: 'main', url: 'https://github.com/SOLDGER96/expt5.git'
            }
        }

        stage('Build') {
            steps {
                // Clean and build the project using Maven
                sh 'javac Pract5.java'
            }
        }

        stage('Test') {
            steps {
                // Run unit tests
                sh 'java Pract5'
            }
        }

    }


}
