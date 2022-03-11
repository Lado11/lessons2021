pipeline {
  agent any
  stages {
    stage('in nodejs') {
      parallel {
        stage('in nodejs') {
          agent any
          steps {
            sleep 5
          }
        }

        stage('in python') {
          steps {
            sleep 5
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