pipeline {
  agent any
  stages {
    stage('STage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo 'Hello PipeLine1'
          }
        }
        stage('Stage2') {
          steps {
            build(job: 'java', quietPeriod: 1)
          }
        }
      }
    }
    stage('Stage3') {
      steps {
        sleep 5
      }
    }
  }
}