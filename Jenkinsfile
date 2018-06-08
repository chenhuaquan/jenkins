pipeline {
  agent any
  stages {
    stage('clean workdir') {
      steps {
        sh '''/home/clean-workdir.sh
'''
      }
    }
    stage('extract files') {
      steps {
        sh '/home/clean-workdir.sh'
      }
    }
    stage('copy files') {
      steps {
        sh '/home/clean-workdir.sh'
      }
    }
  }
}