pipeline {
   agent any
  options { 
    buildDiscarder(logRotator(numToKeepStr: '3')) 
    disableConcurrentBuilds()
  } 
  stages {     
    stage('Stage1') {
      steps {
        sh 'echo stage1'
      }
    }
    
    stage('Printfile') {
      steps {
        sh 'cat abc.txt'
      }
    }
     
      stage('Stage2') {
      steps {
        sh 'echo stage2'
      }
    }
      stage('Stage3') {
      steps {
        sh 'echo stage3'
      }
    }
     
  }
}
