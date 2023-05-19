pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        node('naster'){
          checkout scn
        }
      }
    }

    stage('build') {
      steps {
        node('naster'){
           sh 'echo "connecting"'
        }
      }
    }

  }
  environment {
    APP_ENV = 'production'
  }
}