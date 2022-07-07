pipeline {
  agent none
  stages {
    stage('Update Docker Image') {
      steps {
        echo 'updated docker image nginx'
        publishEvent event:jsonEvent("""
          {
            'image':{'name':'nginx','action':'update','tag':'1.22.0'}
          }
        """), verbose: true
      }
    }
  }
}
