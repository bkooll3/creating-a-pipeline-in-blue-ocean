pipeline {
  agent none
  stages {
    stage('Build') {
      steps {
        echo 'Hello Mod'
      }
    }
    stage('Test') {
      environment {
        CI = 'true'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }
  }
}