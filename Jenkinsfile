pipeline {
  agent any
  stages {
      stage ('Build') {
          steps {
            echo 'Running build automation'
            sh 'chmod 755 ./gradlew'
            sh './gradlew build --no-daemon'
            archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
          }
      }
 }
