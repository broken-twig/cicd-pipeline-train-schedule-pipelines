pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running building automation'
        sh './gradelw build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }  
}
