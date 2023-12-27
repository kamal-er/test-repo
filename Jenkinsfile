pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }

        stage('Run Tests') {
            steps {
                script {
                    sh 'npm test'
                }
            }
        }

        stage('Deploy to Test Server') {
            steps {
                script {
                    // Déployer sur le serveur de test (remplacez avec votre propre script ou commande)
                    sh 'ssh user@test-server "cd /path/to/app && git pull && npm install && pm2 restart app"'
                }
            }
        }
    }
}
