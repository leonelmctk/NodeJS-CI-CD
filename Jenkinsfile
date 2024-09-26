pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/leonelmctk/NodeJS-CI-CD.git'
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
                    // Aquí puedes agregar pasos de construcción como `npm run build`
                    sh 'npm run build' // Suponiendo que tu proyecto use npm para build
                }
            }
        }
    }
