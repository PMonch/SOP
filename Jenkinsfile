pipeline {
    agent { docker { image 'node:10.15.3' } }
    stages {
        stage('build') {
            steps {
                cmd 'npm --version'
            }
        }
    }
}
