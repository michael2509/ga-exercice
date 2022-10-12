pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                cd './node-app'
                nodejs(nodeJSInstallationName: '17.9.1') {
                    sh 'npm install'
                    sh 'npm run build'
                    sh 'npm test'
                }
                echo 'finished'
            }
        }
    }
}