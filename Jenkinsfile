pipeline {
  agent any
  stages {
    stage('step1') {
      steps {
        echo 'hellow blue ocean'
      }
    }
    stage('step') {
      steps {
        sh 'ls'
      }
    }
    stage('build a job') {
      steps {
        build 'testBlueOcean'
      }
    }
  }
}