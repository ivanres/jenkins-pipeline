pipeline {
  agent any
  stages {
    stage('Buid') {
      steps {
        echo 'Building thing!'
        sh 'jenkins/build.sh'
      }
    }

    stage('Test') {
      steps {
        echo 'testing thing!'
        sh 'jenkins/test-all.sh'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying thing!'
        sh 'jenkins/deploy.sh'
      }
    }

  }
}