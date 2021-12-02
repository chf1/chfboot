pipeline {
  agent any
  stages {
    stage('buid java') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('docker build') {
      steps {
        sh 'docker build -t wiljuschkin/chfboot .'
      }
    }

  }
}