pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from repository
                git branch: 'main', url: 'https://github.com/SOLDGER96/expt4.git'
            }
        }

        stage('Build') {
            steps {
                // Clean and build the project using Maven
                bat 'javac Pract5.java'
            }
        }

        stage('Run') {
            steps {
                // Run unit tests
                bat 'java Pract5'
            }
        }

    }


}
