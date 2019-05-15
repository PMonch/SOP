pipeline {
    agent any

    tools {nodejs "versie 10.15.3"}
    stages {
        stage('build') {
            steps {
                sh 'npm start'
            }
        }
    }
}
