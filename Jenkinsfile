pipeline {
  agent { label 'python-agent' }

  stages  {
    stage ('Check python version') {
      steps {
        sh '''
          python3 --version
          whoami
          pwd
          '''
    }
    }
  
     
     stage ('Running the app') {
       steps {
         sh 'python3 app.py'
     }
     }
   
  }
}

  
      
