pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Running first stage'
      }
    stage('Build') {
 steps {
 timeout(time: 3, units: 'MINUTES') {
 retry(5) {
 powershell './flakey-deploy.ps1'
 }
 }
 }
 }
 
  }
}
