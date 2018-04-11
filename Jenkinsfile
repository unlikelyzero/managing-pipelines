pipeline {
  agent any
  stages {
    stage('NPM Build') {
      steps {
        echo 'I\'m Building!'
        sh 'curl http://jenkins.jx.192.168.64.2.nip.io/job/test42demo/job/master/lastBuild/api/json\''
      }
    }
  }
}