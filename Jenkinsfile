pipeline {
  agent any
  stages {
    stage('step1') {
      parallel {
        stage('print message') {
          steps {
            echo 'hellow blue ocean'
          }
        }
        stage('write file') {
          steps {
            writeFile(file: 'work', text: 'build', encoding: 'UTF-8')
          }
        }
      }
    }
    stage('shellscript') {
      steps {
        sh 'll'
      }
    }
    stage('shellscript(rm)') {
      steps {
        sh 'rm -rf work'
      }
    }
    stage('shellscript(ll)') {
      steps {
        sh 'll'
      }
    }
  }
}