pipeline {
  agent any
  stages {
        
    stage  ("Multi step") {
      steps {
        sh 'echo "Running now"'
        sh  'uptime'
        sh 'free -m'
        sh 'python3 app.py'
        sh 'echo "Finished the job"'
      }
    }
  }
}
      
