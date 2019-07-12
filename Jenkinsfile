pipeline {
  agent any
  stages {
    stage('echo Hello') {
      parallel {
        stage('echo Hello') {
          steps {
            sh 'echo "Hello"'
          }
        }
        stage('echo World') {
          steps {
            sh 'echo \'World\''
          }
        }
      }
    }
    stage('print Done') {
      steps {
        echo 'Done done done done!'
      }
    }
  }
}