pipeline {
  agent any
  stages {
    stage('getting maven version') {
      parallel {
        stage('getting maven version') {
          steps {
            sh 'mvn --version'
          }
        }

        stage('compiling maven') {
          steps {
            powershell(script: 'mvn compile', returnStatus: true)
          }
        }

      }
    }

  }
}