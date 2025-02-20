pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo/sample-java-project.git'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment steps here (e.g., copying JAR/WAR to a server)
            }
        }
    }
}

