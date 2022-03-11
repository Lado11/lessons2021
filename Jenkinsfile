pipeline {
  agent any
  stages {
    stage('web server') {
      parallel {
        stage('in nodejs') {
          agent any
          steps {
            sleep 5
          }
        }

        stage('in python') {
          steps {
            sleep 1
            error 'error'
          }
        }

      }
    }

    stage('create') {
      steps {
        sleep 1
      }
    }

  }
}