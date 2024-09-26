pipeline {
    agent {
        docker {
            image 'node:latest'
            args '-u root:root' // Asegúrate de tener permisos necesarios
        }
    }
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        // Otras etapas...
    }
}
