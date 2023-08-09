 pipeline {
  agent //{ dockerfile true }
  { 
 docker {
  image='jenkins/agent'
  registryUrl="https://hub.docker.com"
  registryCredentials='docker_hub_id'
  }
  }
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

