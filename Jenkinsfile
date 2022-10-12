pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'cd "./node-app"'
                nodejs(nodeJSInstallationName: '17.9.1') {
                    sh 'npm install'
                    sh 'npm run build'
                    sh 'npm test'
                }
                sh 'echo "finished"'
            }
        }
    }
}