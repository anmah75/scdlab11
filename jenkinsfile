pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/aditya-sridhar/simple-reactjs-app?tab=readme-ov-file'
            }
        }
        stage('Dependency Installation') {
            steps {
                sh 'npm install'  // Example command for installing dependencies
            }
        }
        stage('Build') {
            steps {
                echo 'docker build -t simple-reactjs-app-master'  // Example command 
            }
        }
        stage('Run') {
            steps {
                sh 'docker run -d -p 8080:80 simple-reactjs-app-master'  
            }
        }
        stage('Push') {
            steps {
                echo 'docker-push'  
            }
        }
        
    }
}

