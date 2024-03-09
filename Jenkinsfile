pipeline{
  agent any

  stages{
    stage('Checkout'){
      steps
      {
      echo "Checkout code from git"
      git url: "https://github.com/ankithaT27/Jenkinspipeline.git" , branch:"master"
      }
    }

    stage('Build'){
      steps
      {
        echo "build docker file"
        sh "docker build . -t my-note-app"
      }
    }

  }
