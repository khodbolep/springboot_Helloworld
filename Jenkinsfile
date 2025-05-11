pipeline {
    agent any

    tools {
        maven 'Maven 3.9.9'   // Change to match your Maven name in Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/khodbolep/springboot_Helloworld.git'
            }
        }

        stage('Build & Unit Test') {
            steps {
                bat 'mvn clean test'
            }
        }
    }
}
