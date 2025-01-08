pipeline {
    agent { docker 'jenkins/jenkins:lts-jdk17' }  // This is the Jenkins Docker container

    stages {
        stage('Setup Python Environment') {
            steps {
                script {
                    sh 'python3 --version'  // Ensure Python is installed
                }
            }
        }
    }
}
