pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
         sh 'gradle wrapper --gradle-version=5.0 --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}

