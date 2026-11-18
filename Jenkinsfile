pipeline {
    agent any

    tools {
        nodejs 'NodeJS22'
    }

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'npm ci'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }

        stage('Build React') {
            steps {
                bat 'npm run build'
            }
        }
    }
}
