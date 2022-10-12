pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: 'Node 18.10.0') {
                    sh 'npm install'
                    sh 'npm run build'
                    sh 'npm test'
                }
            }
        }
    }
}