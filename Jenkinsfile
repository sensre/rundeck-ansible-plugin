pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'sudo docker run -d -p 4440:4440 -e RUNDECK_GRAILS_URL=http://0.0.0.0:4440  --name sensrundeck3 -v rundeck:/home/rundeck/data rundeck:3.2.3'
      }
    }
  }
}