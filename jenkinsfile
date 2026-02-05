pipeline {
    agent {
        docker {
            image 'node:18'
            args '-u root'
        }
    }
    stages {
        stage('Install') {
            steps {
                sh 'node -v'
                sh 'npm -v'
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
