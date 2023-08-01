pipeline {
  agent { dockerfile true }
   triggers {
        pollSCM '* * * * *'
    }
  stages {
    stage('Test') {
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
