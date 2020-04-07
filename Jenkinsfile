pipeline {
  agent {
    docker {
      image 'rundeck'
      args '-p 4440:4440'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'apt-get update -y'
      }
    }
  }
}