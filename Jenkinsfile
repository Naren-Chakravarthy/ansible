pipeline {
  agent any
    options {
      ansiColor('xterm')
    }
    stages {
      stage("Do a dry run") {
        steps {
          sh ''' ansible-playbook roboshop.yml -e HOST=localhost -e role_name=frontend -C '''
        }
      }
    }
}