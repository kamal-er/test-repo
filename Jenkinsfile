pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Étape pour récupérer le code à partir du référentiel Git
                git 'https://github.com/votre-utilisateur/votre-projet.git'
            }
        }
        stage('Build') {
            steps {
                // Étape de construction simple, par exemple, exécuter un script shell
                sh './build.sh'
            }
        }
    }
}
