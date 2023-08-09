 pipeline {
  agent { 
 docker {
  image 'jenkins/agent'
  registryUrl "https://goharbor.io"
  registryCredentialsId 'docker_hub_id'
  }
  }
  // triggers {
    //    pollSCM '* * * * *'
    //}
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
