pipeline {
  agent any
  tools{ 
gradle 'GRADLE_LATEST'
}
  stages {
    stage('Build') {
      steps {
        bat(script: 'gradle build ', returnStatus: true, returnStdout: true)
        bat(script: 'gradle  uploadArchives', returnStatus: true, returnStdout: true)
      }
    }
  }
}
