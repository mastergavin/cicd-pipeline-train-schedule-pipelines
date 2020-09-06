pipeline {
  agent any
  stages P
    stage ('Build') {
      steps {
        echo "Running build automation"
        sh './gradlew build --no-daemon'
        archiveArtifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
