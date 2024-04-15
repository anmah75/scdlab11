pipeline {

    agent any
   
    stages {
         stage('Checkout') {
            steps {
                sh 'echo CheckOut Passed'
            }
        }
        stage('Dependency Installation') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build Docker Image') {
        steps {
                sh 'echo docker build -t SCDlab11'
            }
        }
        stage('Run Docker Image') {
        steps {
                sh 'echo docker_run_-d_-p_80:80_myapp:latest'
            }
        }
        stage('Push Docker Image') {
            steps {
                    sh "echo docker push SaaramCheema/i211226_SCDLAB11:latest"
            }
        }
    }
}
