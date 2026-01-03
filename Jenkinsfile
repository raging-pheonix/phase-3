pipeline {
  agent any
  stages ("Multi step") {
    stage {
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
      
