pipeline {
  agent any
  stages {
    
    stage('build') {
      steps {
        input(id: 'userinput', message: 'enter ep', ok: 'ok', parameters: [string(defaultValue: '', description: '', name: 'endpoint')])
        echo $endpoint
      }
    }
  }
}
