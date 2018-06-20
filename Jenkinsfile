pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                echo "Hello Jenkins"
                sh 'npm install'
                sh './node_modules/.bin/eslint index.js'
            }
        }
    }
    post {
        success {
            slackSend color: "#3399ff", channel:"#test-jenkins", message: "build successfully"
        }
        failure {
            slackSend color: "#ff3366", channel:"#test-jenkins", message: "build failed"
        }
    }
}