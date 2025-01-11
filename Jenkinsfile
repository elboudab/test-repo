pipeline {
  agent none
  stages {
    stage('start') {
      steps {
        echo 'start '
      }
    }

    stage('check ip') {
      steps {
        sh 'ifconfig'
      }
    }

    stage('finish') {
      steps {
        echo 'Finished'
      }
    }

  }
}