pipeline {
    agent {
            docker { image 'node:7-alpine' }
        }

    stages {
        stage('Build') {
            agent any
            steps {
                checkout scm
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