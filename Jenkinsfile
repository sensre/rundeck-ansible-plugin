pipeline {
  agent {
    docker {
      image 'rundeck:3.2.3'
      args '-p 4440:4440'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'docker run -d -p 4440:4440 -e RUNDECK_GRAILS_URL=http://172.31.56.113:4440  --name sensrundeck3 -v rundeck:/home/rundeck/data rundeck/rundeck:3.2.3'
      }
    }

  }
}