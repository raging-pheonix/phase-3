pipeline {
  agent { label 'python-agent' }

  stages ('Check python version') {
    stage {
      steps {
        sh '''
          python3 --version
          whoami
          pwd
          '''
    }
    }
  }
   stages ('Running the app') {
     stage {
       steps {
         sh 'python3 app.py'
     }
     }
   }
}

  
      
