pipeline {
  agent { label 'host' }
  // agent {
  //     docker {
  //         image 'maven:3-alpine'
  //         label 'host'
  //     }
  // }
  stages {
    stage('Example') {
      steps {
        sh 'docker --version'
        echo 'Hello World'
      }
    }
  }
  post {
    always {
      echo 'I will always say Hello again!'
    }
  }
}
