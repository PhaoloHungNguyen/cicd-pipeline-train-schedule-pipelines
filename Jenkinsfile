pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        echo 'Then create configuration file'
        echo 'Then create configuration file' > configuration.txt
        echo 'After create configuration file'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
