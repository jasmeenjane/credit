pipeline {
    agent any
    environment {
        STAGING_SERVER = 'staging.example.com'
        PROD_SERVER = 'prod.example.com'
        EMAIL = 'jasmeen4873.be23@chitkara.edu.in'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                echo "Could Use NPM or MVN"
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit tests...'
                echo "hello"
                
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Performing code analysis...'
                
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Running security scan...'
                
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to Staging...'
                
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging...'
                
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to Production...'
                
            }
        }
    }
    post {
        always {
            emailext (
                subject: "Jenkins Pipeline Execution",
                body: "Pipeline execution complete. Check Jenkins for details.",
                to: "$EMAIL"
            )
        }
    }
}
