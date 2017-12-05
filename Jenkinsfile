pipeline {
  agent any
  stages {
    stage('Get Source') {
      steps {
        git(url: 'https://github.com/joanbaez/APItest.git', branch: 'master', credentialsId: 'GitHubCredentials')
      }
    }
    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            sleep 1
          }
        }
        stage('1') {
          steps {
            sleep 1
          }
        }
        stage('2') {
          steps {
            sleep 1
          }
        }
        stage('3') {
          steps {
            sleep 1
          }
        }
      }
    }
    stage('stage2') {
      parallel {
        stage('stage2') {
          steps {
            bat '1'
          }
        }
        stage('4') {
          steps {
            sleep 1
          }
        }
      }
    }
    stage('5') {
      steps {
        sleep 1
      }
    }
    stage('6') {
      steps {
        sleep 1
      }
    }
  }
}