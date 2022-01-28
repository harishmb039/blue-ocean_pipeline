pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''ls
pwd'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'print message'
          }
        }

        stage('test1') {
          steps {
            echo 'print message'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sleep 5
      }
    }

  }
}