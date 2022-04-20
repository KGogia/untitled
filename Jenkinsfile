pipeline {
  agent any
  stages {
    stage('Log Maven') {
      parallel {
        stage('Log Maven') {
          steps {
            sh 'mvn --version'
          }
        }

        stage('Run Test') {
          steps {
            sh 'mvn compile test package'
          }
        }

      }
    }

  }
}