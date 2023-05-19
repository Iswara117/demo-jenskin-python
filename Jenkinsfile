pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        git(credentialsId: 'credentials-python-jenkins', url: 'git@github.com:Iswara117/demo-jenskin-python.git', branch: 'main')
      }
    }

    stage('build') {
      steps {
        sh 'echo "connecting"'
      }
    }

  }
  environment {
    APP_ENV = 'production'
  }
}