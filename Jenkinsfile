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
         sh 'sudo npm install'  
      }
    }
    
    stage('Test') {
      steps {
         sh 'sudo npm test'
         sh 'sudo npm run test:e2e'  
        
      }
    }
  }
}
