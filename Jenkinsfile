pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        echo 'compile'
      }
    }
    stage('unit test') {
      parallel {
        stage('unit test') {
          steps {
            echo 'unit test'
          }
        }
        stage('UI test') {
          steps {
            echo 'UI test'
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