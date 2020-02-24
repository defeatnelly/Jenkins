pipeline {
    agent {
            docker { image 'node:7-alpine' }
        }
        
    stages {
        stage('Build') {

            agent{
                checkout scm
            }
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'node --version'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}