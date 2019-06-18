pipeline {
  agent any
  stages {
    stage('Change Endpoint') {
      steps {
        input(message: 'Enter endpoint', id: 'ep', ok: 'ok', submitter: 'ep')
      }
    }
  }
}