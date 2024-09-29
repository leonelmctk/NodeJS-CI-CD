pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
               git branch: 'main' url: 'https://github.com/leonelmctk/NodeJS-CI-CD.git', credentialsId: 'github-credentials'   
            }
        }
        stage('Install Dependencies') {
            steps {
                script {
                    echo 'Installing dependencies...'
                    sh 'npm install'
                }
            }
        }
        stage('Run Tests') {
            steps {
                script {
                    echo 'Running tests...'
                    sh 'npm test'
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    echo 'Building the application...'
                    // Agregar cualquier paso de construcción necesario
                }
            }
        }
    }
}
