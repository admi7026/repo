pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Build the code using Maven
                echo 'Building code using Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                // Run unit tests and integration tests using testing tools
                echo 'Running unit and integration tests'
            }
        }
        stage('Code Analysis') {
            steps {
                // Integrate a code analysis tool (e.g., SonarQube) to analyze the code
                echo 'Analyzing code using SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                // Perform a security scan using a security scanning tool
                echo 'Performing security scan'
            }
        }
        stage('Deploy to Staging') {
            steps {
                // Deploy application to staging server (e.g., AWS EC2)
                echo 'Deploying to staging server'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                // Run integration tests on staging environment
                echo 'Running integration tests on staging environment'
            }
        }
        stage('Deploy to Production') {
            steps {
                // Deploy application to production server (e.g., AWS EC2)
                echo 'Deploying to production server'
            }
        }
    }
    
    post {
        success {
            // Send email notification on success
            emailext body: "Pipeline successful", subject: "Pipeline Success", to: "hplapi62@gmail.com"
        }
        failure {
            // Send email notification on failure
            emailext body: "Pipeline failed", subject: "Pipeline Failure", to: "hplapi62@gmail.com"
        }
    }
}
