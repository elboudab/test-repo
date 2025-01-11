pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'printing ip address'
          }
        }

        stage('check ip') {
          steps {
            sh 'ifconfig'
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'test'
      }
    }

    stage('deploy') {
      steps {
        sh '''docker run -d alpine sh -c "while true; do echo Hello Alpine; sleep 5; done"
'''
      }
    }

    stage('') {
      steps {
        echo 'Finish steps'
      }
    }

  }
}