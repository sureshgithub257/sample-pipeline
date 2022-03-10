pipeline {
  agent any
  stages {
    stage('Notice') {
      steps {
        sh 'echo Running first stage'
      }
    }
    stage('Build') {
      steps {
        timeout(time: 3, unit: 'MINUTES') {
          retry(5) {
            powershell './flakey-deploy.ps1'
          }
       }
     }
   }
 
  }
}


