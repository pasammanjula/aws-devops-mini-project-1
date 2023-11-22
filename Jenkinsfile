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
        "sh mvn validate"
      }
    }
    stage('compile') {
      steps {
        "sh mvn compile"
      }
    }
    stage('test') {
      steps {
        "sh mvn test"
      }
    }
    stage('deploy') {
      steps {
        "sh mvn package"
      }
    }
  }
}
