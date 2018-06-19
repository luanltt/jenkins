pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                echo "Hello Jenkins"
                sh 'printenv'
                sh 'ls -l'
            }
        }
    }
}