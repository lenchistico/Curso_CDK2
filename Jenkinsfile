pipeline {
  agent any
  stages {
    stage('Inicio') {
      steps {
        echo 'Inicializando'
        sleep 2
      }
    }

    stage('Build') {
      parallel {
        stage('Tools Information') {
          steps {
            sh 'node --version'
          }
        }

        stage('Check FS') {
          steps {
            sh 'ls -ltr'
          }
        }

      }
    }

  }
}