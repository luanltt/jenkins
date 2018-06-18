pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                echo "Build number: ${env.BUILD_NUMBER}"
                echo "Build Name: ${env.BRANCH_NAME}"
                echo "Change ID: ${env.CHANGE_ID}"
                sh 'npm --version'
            }
        }
    }
}