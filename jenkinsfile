pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from repository
                git branch: 'main', url: 'https://github.com/Atharv-Bandekar/pract5.git'
            }
        }

        stage('Build') {
            steps {
                // Clean and build the project using Maven
                bat 'javac Pract5.java'
            }
        }

        stage('Test') {
            steps {
                // Run unit tests
                bat 'java Pract5'
            }
        }

    }


}
