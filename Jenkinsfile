pipeline {
  agent any
  stages {
    stage('initial') {
      steps {
        parallel(
          "step 1": {
            sh 'echo "1"'
            
          },
          "step 2": {
            sh 'echo "2"'
            
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