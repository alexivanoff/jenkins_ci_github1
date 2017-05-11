pipeline {
  agent any
  stages {
    stage('initial') {
      steps {
        parallel(
          "step 1": {
            sh 'pwd'
            
          },
          "step 2": {
            sh 'ls'
            
          }
        )
      }
    }
    stage('tada') {
      steps {
        sh 'echo "tada"'
      }
    }
  }
}