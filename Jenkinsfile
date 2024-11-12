pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat './mvnw clean package'
            }
        }
        stage('Test') {
            steps {
                bat './mvnw test'
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
