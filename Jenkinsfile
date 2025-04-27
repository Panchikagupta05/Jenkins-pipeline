pipeline {
    agent any
    stages {
        stage('Scripted Pipeline Inside Declarative') {
            steps {
                script {
                    stage('Inner Scripted: Checkout Code') {
                        checkout scm
                    }
                    stage('Inner Scripted: Build') {
                        echo "Building the project..."
                    }
                    stage('Inner Scripted: Test') {
                        echo "Running tests..."
                    }
                    stage('Inner Scripted: Deploy') {
                        echo "Deploying the project..."
                    }
                }
            }
        }
    }
}
