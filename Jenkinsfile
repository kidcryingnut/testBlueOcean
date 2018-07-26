pipeline {
  agent any
  stages {
    stage('step1') {
      parallel {
        stage('step1') {
          steps {
            echo 'hellow blue ocean'
          }
        }
        stage('step1-1') {
          steps {
            writeFile(file: 'work', text: 'build', encoding: 'UTF-8')
          }
        }
        stage('step1-2') {
          steps {
            sleep 5
          }
        }
      }
    }
    stage('step') {
      steps {
        sh 'ls'
      }
    }
  }
}