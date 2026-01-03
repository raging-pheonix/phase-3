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

    stage ("Create a file") {
      steps {
        sh 'echo "Heeloo from mastery" > p-file.txt'
      }
    }

    stage ("Accessing the file") {
      steps {
        sh 'cat p-file.txt'
      }
    }
  }
}
      
