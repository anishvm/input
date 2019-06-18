pipeline {
  agent any
  stages {
    stage('Change Endpoint') {
      steps {
        input(id: 'userinput', message: 'enter ep', ok: 'ok', parameters: [string(defaultValue: '', description: '', name: 'endpoint')])
      }
    }
    stage('build') {
      steps {
        sh 'echo $userinput.Env'
      }
    }
  }
}