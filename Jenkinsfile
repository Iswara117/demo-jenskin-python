pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        node('master'){
          checkout scm
        }
      }
    }

    stage('build') {
      steps {
        node('master'){
           sh 'echo "connecting"'
        }
      }
    }

  }
  environment {
    APP_ENV = 'production'
  }
}