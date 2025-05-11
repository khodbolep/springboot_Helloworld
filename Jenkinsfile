pipeline {
    agent any

    tools {
        maven 'Maven 3.8.5'   // Change to match your Maven name in Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/your-username/your-repo-name.git'
            }
        }

        stage('Build & Unit Test') {
            steps {
                bat 'mvn clean test'
            }
        }
    }
}
