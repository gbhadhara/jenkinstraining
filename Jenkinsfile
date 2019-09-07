pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo 'Hello pipeline 1 '
          }
        }
        stage('Stage 2') {
          steps {
            build(job: 'buildjob1', quietPeriod: 2)
          }
        }
      }
    }
    stage('Blue Stage 1') {
      steps {
        sleep 1
      }
    }
  }
}