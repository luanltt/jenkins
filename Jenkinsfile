pipeline {
  agent {
    docker {
      image 'node:6.3'
    }

  }
  stages {
    stage('build') {
      steps {
        echo sh(returnStdout: true, script: 'env')
        sh 'printenv'
        echo sh(script: 'env|sort', returnStdout: true)
      }
    }
  }
}