pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'Hello mostafa .... '
      }
    }
    
     stage('Install dependencies') {
      steps {
         sh 'ls -la'  
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
