pipeline {
  agent {
    node {
      label 'node'
    }
    
  }
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'sleep 1'
            sleep 1
          }
        }
        stage('stage1-1') {
          steps {
            sleep 1
          }
        }
        stage('stage1-2') {
          steps {
            sleep 1
          }
        }
      }
    }
    stage('stage2') {
      steps {
        sleep 1
      }
    }
  }
  environment {
    key = 'value'
  }
}