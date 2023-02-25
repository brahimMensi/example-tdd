pipeline {
  agent any
  tools {
    maven 'maven3'
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn -Dversion=3 compile'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn -Dversion=3 test'
      }
    }
    stage('Install') {
      steps {
        sh 'mvn -Dversion=3 install'
      }
    }
  }
}
