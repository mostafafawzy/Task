pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'Hello World .... 7 '
      }
    }
    
     stage('Install dependencies') {
      when {
                branch 'master'
      }
      steps {
         sh 'npm install'  
      }
    }
    
    stage('Test') {
      when {
                branch 'master'
      }
      steps {
         sh 'npm test'
         sh 'npm run test:e2e'        
      }
    }
  }
}
