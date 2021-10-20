pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'hello from the trigger'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploy to prod'
      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}