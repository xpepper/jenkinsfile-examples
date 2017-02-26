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
        withEnv(["PATH+DOCKER=/usr/local/bin"]) {
           sh 'docker --version'
         }
        // env.PATH = "/usr/local/bin:${env.PATH}"
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
