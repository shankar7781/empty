pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd

date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test run'
          }
        }

        stage('test parallel') {
          steps {
            echo 'test parallel'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}