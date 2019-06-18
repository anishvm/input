pipeline {
  def userinput =  timeout(time:60, unit:'SECONDS') {input(
     id: 'userinput', message: 'URL Required', parameters: [
     [$class: 'TextParameterDefinition', defaultValue: '', description: 'URL', name: 'url'],
    ])
  }
  agent any
  stages {
    stage('Change Endpoint') {
      steps {
        input(id: 'userinput', message: 'enter ep', ok: 'ok', parameters: [string(defaultValue: '', description: '', name: 'endpoint')])
      }
    }
    stage('build') {
      steps {
        sh "echo userinput"
      }
    }
  }
}
