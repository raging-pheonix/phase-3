pipeline {
  agent any
  
  environment {
    APP_EN = 'developer'
    FRT_PB = 'fruity pebbles'
  }
    
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

    stage ("Printing environment variables") {
      steps {
        sh 'echo app = $APP_EN'
        sh 'echo fruit =$FRT_PB'
      }
    }

    stage ("Workspace variable") {
      steps {
        sh 'echo Current Workspace is $WORKSPACE'
        sh 'ls $WORKSPACE'
      }
    }
  }
}
      
