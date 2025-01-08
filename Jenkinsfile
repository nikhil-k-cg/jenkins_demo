pipeline {
    agent any  // No Docker container is used
    stages {
        stage('Build') {
            steps {
                script {
                    // Running on the Jenkins host, not in Docker
                    sh 'python3 --version'
                }
            }
        }
    }
}
