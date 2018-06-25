pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        echo 'Initialize variables'
      }
    }
    stage('Checkout') {
      steps {
        sh 'echo " git clone hhtps "'
      }
    }
    stage('Build1') {
      parallel {
        stage('Build1') {
          steps {
            echo 'build 30%'
          }
        }
        stage('Build2') {
          steps {
            echo 'Build 20%'
          }
        }
        stage('Build3') {
          steps {
            echo 'Build 25%'
          }
        }
        stage('Build4') {
          steps {
            echo 'Build 15%'
          }
        }
        stage('Build5') {
          steps {
            echo 'build 10%'
          }
        }
      }
    }
    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'test 50%'
          }
        }
        stage('Test2') {
          steps {
            echo 'test 30%'
          }
        }
        stage('Test3') {
          steps {
            echo 'test 20%'
          }
        }
      }
    }
    stage('Release') {
      steps {
        echo 'release successfully'
      }
    }
  }
}