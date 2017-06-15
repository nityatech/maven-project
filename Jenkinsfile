pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        parallel(
          "build": {
            pwd(tmp: true)
            
          },
          "test": {
            echo 'Test'
            
          }
        )
      }
    }
    stage('junk') {
      steps {
        input(message: 'WAit', id: 'Wait', ok: 'Yes')
      }
    }
  }
}