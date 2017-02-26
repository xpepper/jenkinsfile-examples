pipeline {
  agent { label 'osx' }
  // agent {
  //     docker {
  //         image 'maven:3-alpine'
  //         label 'host'
  //     }
  // }
  stages {
    stage('Example') {
      steps {
        env.PATH = "/usr/local/bin:${env.PATH}"
        sh 'docker --version'
      }
    }
  }
  post {
    always {
      echo 'I will always say Hello again!'
    }
  }
}
