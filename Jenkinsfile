pipeline {
  agent {
    docker { image 'node:16-alpine' }
  }
  stages {
    stage('Deploy') {
      steps {
        sh 'node --version'
      }
    }
  stage('Test'){
     steps {
       echo "hi"
  }
  }
}
}
