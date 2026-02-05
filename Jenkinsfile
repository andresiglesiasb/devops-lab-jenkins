pipeline {
    agent any

    options {
        buildDiscarder(logRotator(numToKeepStr: '10'))
        timeout(time: 1, unit: 'HOURS') 
    }

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
