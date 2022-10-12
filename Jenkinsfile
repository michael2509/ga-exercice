pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: '18.10') {
                    sh 'npm install'
                    sh 'npm run build'
                    sh 'npm test'
                }
            }
        }
    }
}