pipeline {
  agent any
  stages {
    stage('initial') {
      steps {
        parallel(
          "step 1.1": {
            sh 'pwd'
            
          },
          "step 1.2": {
            sh 'ls'
            
          },
          "step1.3": {
            build(job: 'jenkins-ci2', parameters: [[$class: 'StringParameterValue', name: 'FOLDER', value: "/var"]], wait: true)
            
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
