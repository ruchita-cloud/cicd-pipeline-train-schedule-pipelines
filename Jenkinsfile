pipeline{
  agent any
  stages{
    stage('Build')
    {
      steps{
        echo 'Running code Build'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/tainSchedule.zip'
      }
    }
  }
}
