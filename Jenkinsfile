pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'Hello World .... '
      }
    }
    
     stage('Install dependencies') {
      steps {
         sh 'npm install'  
      }
    }
    
    stage('Test') {
      steps {
         sh 'npm test'
         sh 'npm run test:e2e'        
      }
    }
  }
}
