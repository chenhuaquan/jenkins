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
    stage('regression test') {
      steps {
        sh '/home/clean-workdir.sh'
      }
    }
    stage('completed') {
      parallel {
        stage('Completed') {
          steps {
            sh '/home/clean-workdir.sh'
          }
        }
        stage('file is not ready: email project manager') {
          steps {
            sh '/home/clean-workdir.sh'
          }
        }
        stage('copy file fails: email support engineer') {
          steps {
            sh '/home/clean-workdir.sh'
          }
        }
        stage('regression test fails: contact test lead') {
          steps {
            sh '/home/clean-workdir.sh'
          }
        }
      }
    }
  }
}