pipeline {
  agent { dockerfile true }
   triggers {
        pollSCM '* * * * *'
    }
  stages {
    stage('Tzzettttst') {
      steps {
        sh '''
          node --version
          git --version
          curl --version
        '''
      }
    }
  }
}
