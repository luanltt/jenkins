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
}