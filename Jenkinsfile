pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "npm install'
                sh 'npm run build'
                sh 'npm test'
            }
        }
    }
}