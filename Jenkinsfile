pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo 'Hello PipeLine1'
          }
        }
        stage('Haha') {
          steps {
            echo 'Stage2 job'
          }
        }
      }
    }
    stage('Stage3') {
      parallel {
        stage('Stage3') {
          steps {
            sleep 5
          }
        }
        stage('PrintMsg') {
          steps {
            echo 'haha2'
          }
        }
      }
    }
  }
}