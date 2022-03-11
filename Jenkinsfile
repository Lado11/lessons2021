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
            node(label: 'sd')
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