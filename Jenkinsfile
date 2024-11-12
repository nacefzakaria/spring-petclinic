pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/nacefzakaria/spring-petclinic.git'
            }
        }
        stage('Build') {
            steps {
                sh './mvnw clean package'
            }
        }
        stage('Test') {
            steps {
                sh './mvnw test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Replace this with actual deployment commands if needed
            }
        }
    }
}
