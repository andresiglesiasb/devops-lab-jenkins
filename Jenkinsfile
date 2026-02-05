pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '--- Starting Build Stage ---'
                echo 'Compiling source code...'
            }
        }
        stage('Test') {
            steps {
                echo '--- Starting Unit Tests ---'
                echo 'All tests passed successfully.'
            }
        }
        stage('Deploy') {
            steps {
                echo '--- Deploying to Staging Environment ---'
                echo 'Deployment completed successfully.'
            }
        }
    }
}
