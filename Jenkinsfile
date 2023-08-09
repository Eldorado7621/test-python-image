pipeline {
  agent { dockerfile true }
   triggers {
        pollSCM '* * * * *'
    }
  stages {
    stage('Tzzest') {
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
