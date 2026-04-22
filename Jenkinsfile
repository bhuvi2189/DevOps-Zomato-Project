pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/bhuvi2189/DevOps-Project-Zomato-Kastro.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('OWASP Scan') {
            steps {
                sh './dependency-check.sh --scan . || true'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t zomato-app .'
            }
        }

        stage('Trivy Scan') {
            steps {
                sh 'trivy image zomato-app || true'
            }
        }

        stage('Run Container Test') {
            steps {
                sh 'docker run -d -p 3000:3000 zomato-app || true'
            }
        }
    }
}