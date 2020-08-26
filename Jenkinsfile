pipeline {
  agent {
    docker {
      image 'php:5.6-apache'
    }

  }
  stages {
    stage('build') {
      steps {
        sh '$(aws ecr get-login --no-include-email --region $AWS_DEFAULT_REGION)'
      }
    }

  }
}