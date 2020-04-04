pipeline {
  agent {
    docker {
      args '-p 4440:4440'
      image 'sens/rundeck:3.2.3'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'docker run -d -p 4440:4440 -e RUNDECK_GRAILS_URL=http://172.31.56.113:4440  --name sensrundeck3 -v rundeck:/home/rundeck/data sens/rundeck:3.2.3'
      }
    }

  }
}