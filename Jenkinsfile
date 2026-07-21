pipeline {
    agent { label "linux" }
    stages {
        stage('Checkout') {
            steps { 
              checkout scm
            }
        }
        stage('Build') {
            steps { 
              sh 'npm install'
            }
        }
        stage('Test') {
            steps { 
              echo 'No tests yet'
            }
        }
        stage('Docker Build') {
            steps { 
            sh 'docker build -t demo-app:$BUILD_NUMBER .'
            }
        }
    }
}
