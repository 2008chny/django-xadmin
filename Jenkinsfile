pipeline {
  agent any
  stages {
    stage('A') {
      parallel {
        stage('A') {
          steps {
            sh 'echo "A01"'
            echo 'A02'
          }
        }
        stage('B') {
          steps {
            echo 'B0'
          }
        }
        stage('C') {
          steps {
            input 'C0'
          }
        }
      }
    }
    stage('A1') {
      parallel {
        stage('A1') {
          steps {
            echo 'A1'
          }
        }
        stage('B1') {
          steps {
            echo 'B1'
          }
        }
      }
    }
    stage('A2') {
      steps {
        echo 'A2'
      }
    }
  }
}