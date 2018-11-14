pipeline {
  agent any
  stages {
    stage('pre-check') {
      steps {
        echo 'Hello first pipeline'
        sh 'env'
      }
    }
    stage('build') {
      steps {
        sh 'git status'
        pwd()
        cleanWs(cleanWhenSuccess: true)
      }
    }
  }
}