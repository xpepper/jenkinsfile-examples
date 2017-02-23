pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            label 'host'
        }
    }
    stages {
        stage('Example') {
            steps {
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
