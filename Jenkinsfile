pipeline {
    agent { dockerfile {image 'node:10.15.3' } }
    stages {
        stage('build') {
            steps {
                cmd 'npm --version'
            }
        }
    }
}
