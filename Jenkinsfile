pipeline {
  agent any 
  stages {
    stage ('Build') {
      steps {
        echo "Building the build via gradle"
        sh "./gradlew build"
        archiveArtifacts artifact: 'dist/trainSchedule.zip', fingerprint: true 
      }
    }
