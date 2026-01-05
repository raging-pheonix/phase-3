pipeline {
  agent { label 'python-agent' }

  stages ('Check python version') {
    steps {
      sh '''
        python3 --version
        whoami
        pwd
        '''
    }
  }
   stages ('Running the app') {
     steps {
       sh 'python3 app.py'
     }
   }
}

  
      
