pipeline {
  agent any
  stages {
    stage('Change Endpoint') {
      steps {
        input(id: 'Ep', message: 'enter ep', ok: 'ok', parameters: [string(defaultValue: '', description: '', name: 'endpoint', trim: true)])
      }
    }
    stage('build') {
      steps {
        sh 'echo $endpoint'
      }
    }
  }
}