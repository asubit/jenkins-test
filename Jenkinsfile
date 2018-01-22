pipeline {
  agent any
  stages {
    stage('Build') {
      environment {
        Prod = 'local.lms.dev'
      }
      steps {
        echo 'Building..'
        git(poll: true, url: 'https://github.com/asubit/lms', branch: 'master')
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
}