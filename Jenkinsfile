pipeline {
    agent any
    stages {
        stage('Example clean') {
            steps {
                bat "git clone https://github.com/pknowledge/my-app.git"
                bat "mvn clean my-app"
            }
        }
        stage('Example install') {
            steps {
                sh "mvn install my-app"
            }
        }
        stage('Example test') {
            steps {
                sh "mvn test my-app"
            }
        }
        stage('Example package') {
            steps {
                sh "mvn package my-app"
            }
        }
    }
}
