pipeline {
  agent any
  stages {
    stage('sonar') {
      steps {
        waitForQualityGate true
      }
    }

    stage('status') {
      steps {
        build 'test'
      }
    }

  }
}