pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'echo "Running build on Jenkins container..."'  // Run inside Jenkins container (default behavior)
            }
        }

        stage('Execute on Host Machine') {
            steps {
                echo 'Executing code on the host machine outside the Jenkins container...'
                // Running a shell command on the host machine (outside Docker container)
                sh '''
                    python3 --version
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying project...'
                sh 'echo "Running deployment..."'
            }
        }
    }
}
