pipeline {
  agent any
    stages {
      stage('Build'){
        steps{
          sh 'g++ hello.cpp'
          echo 'Build Stage Successful'
        }
      }
      stage('Test'){
        steps {
          sh './a.out'
          echo 'Test Stage Successful'
        }
      }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
