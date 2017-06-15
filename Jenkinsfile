pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        parallel(
          "build": {
            pwd(tmp: true)
            
          },
          "": {
            echo 'Test'
            
          }
        )
      }
    }
    stage('') {
      steps {
        input(message: 'WAit', id: 'Wait', ok: 'Yes')
      }
    }
  }
}