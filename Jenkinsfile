pipeline {
  agent any 
  stages {
    stage ('Build') {
      steps {
        echo "Building the build via gradle"
        sh "./gradlew build --no-daemon"
        archiveArtifacts artifacts: 'dist/trainSchedule.zip', fingerprint: true 
      }
    }
  }
}
