pipeline {
    agent { docker {image 'node:10.15.3' } }
    stages {
        stage('build') {
            steps {
                bat 'npm --version'
            }
        }
    }
}
