pipeline {
  agent any

  stages {
    stage('checkout') {
      steps {
        checkout scm
      }
    }

    stage('validate') {
      steps {
        "mvn validate"
      }
    }
    stage('compile') {
      steps {
        "mvn compile"
      }
    }
    stage('test') {
      steps {
        "mvn test"
      }
    }
    stage('deploy') {
      steps {
        "mvn package"
      }
    }
  }
}
