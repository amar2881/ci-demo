pipeline {
   agent any
  options { 
    buildDiscarder(logRotator(numToKeepStr: '2')) 
    disableConcurrentBuilds()
  }
  triggers {
       pollSCM('*****')
  }
  
  stages {
    stages('Declarative Checkout') {
      steps {
        checkout scm
      }
    }
    
    stage('Printfile') {
      steps {
        sh 'cat abc.txt'
      }
    }
  }
}
