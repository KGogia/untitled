pipeline {
  agent any
  stages {
    stage('Log Maven') {
      parallel {
        stage('Log Maven') {
          steps {
            powershell(script: 'mnv --version', returnStatus: true)
          }
        }

        stage('Run') {
          steps {
            bat 'mvn clean test'
          }
        }

      }
    }

  }
}