pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: '17.9.1') {
                    cd './node-app'
                    sh 'npm install'
                    sh 'npm run build'
                    sh 'npm test'
                    echo 'finished'
                }
            }
        }
    }
}