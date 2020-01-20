pipeline {
  agent any
  stages {
    stage('Clean') {
      steps {
        sh 'mvn clean'
      }
    }

    stage('Build') {
      steps {
        sh 'mvn clean package -DskipMunitTests'
      }
    }

    stage('Print message') {
      steps {
        echo 'Build Successfull'
      }
    }

  }
}