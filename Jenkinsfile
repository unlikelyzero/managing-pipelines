pipeline {
  agent any
  stages {
    stage('NPM Build') {
      steps {
        echo 'I\'m Building!'
      }
    }
    stage('Run the Units tests') {
      steps {
        echo 'Unit tests!'
      }
    }
    stage('Built For QA') {
      steps {
        sleep 4
      }
    }
    stage('UI Tests') {
      parallel {
        stage('UI Tests') {
          steps {
            sleep 4
          }
        }
        stage('Chrome') {
          steps {
            sleep 4
          }
        }
        stage('IE11') {
          steps {
            sh 'exit 0'
          }
        }
        stage('FireFox Stage') {
          steps {
            sleep 4
          }
        }
      }
    }
    stage('Report') {
      steps {
        echo 'Reported!'
      }
    }
    stage('Deployment') {
      steps {
        sleep 2
      }
    }
  }
}
