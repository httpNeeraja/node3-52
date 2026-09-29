pipeline {
    agent any

    tools {
        nodejs 'NodeJS'
    }

    stages {

        stage('Check Node') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }

        stage('Run') {
            steps {
                sh 'npm start'
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
