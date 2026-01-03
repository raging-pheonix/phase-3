pipeline {
  agent any
  stages {
    
    stage  ("git cloning") {
      steps {
        sh 'echo "Cloning the repo"'
        sh 'git clone https://github.com/raging-pheonix/phase-3.git'
      }
    }
        
    stage  ("Multi step") {
      steps {
        sh 'echo "Running now"'
        sh  'uptime'
        sh 'free -m'
        sh 'python app.py'
        sh 'echo "Finished the job"'
      }
    }
  }
}
      
