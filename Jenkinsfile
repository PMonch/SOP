pipeline {
    agent { docker { image 'node:10.15.3' } }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
        stage('SonarQube Analysis'){
            environment {
                scannerHome = '/var/lib/jenkins/tools/hudson.plugins.sonar.SonarRunnerInstallation/SonarQube_Scanner_3.3.0.1492/bin'
            }
            steps{
                withSonarQubeEnv('sonarqube') {
                    sh '${scannerHome}/bin/sonar-scanner'
                }
            }
        }
    }
}
