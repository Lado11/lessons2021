pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/lessons2021/VladimirBaghdasaryan.git', branch: 'main', changelog: true, poll: true)
      }
    }

    stage('Run Test') {
      parallel {
        stage('Run Test') {
          steps {
            git(url: 'https://github.com/lessons2021/VladimirBaghdasaryan.git', branch: 'main')
          }
        }

        stage('Test of linux') {
          agent any
          steps {
            git(url: 'https://github.com/lessons2021/VladimirBaghdasaryan.git', branch: 'main')
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        git(url: 'https://github.com/lessons2021/VladimirBaghdasaryan.git', branch: 'main')
      }
    }

    stage('End') {
      steps {
        git(url: 'https://github.com/lessons2021/VladimirBaghdasaryan.git', branch: 'main')
      }
    }

  }
}