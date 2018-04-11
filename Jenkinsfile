pipeline {
  agent any
  stages {
    stage('NPM Build') {
      steps {
        echo 'I\'m Building!'
      }
    }
    stage('UI Regression Tests') {
      parallel {
        stage('Chrome') {
          steps {
            sleep 3
          }
        }
        stage('Firefox') {
          steps {
            sleep 4
          }
        }
        stage('IE11') {
          steps {
            sleep 8
            sh 'exit 1'
          }
        }
      }
    }
    stage('Send notifications') {
      steps {
        echo 'HOOOORAY'
      }
    }
  }
}