pipeline {
  agent any 
  stages {
    stage('hello echo') {
      steps {

        echo 'HELLO'

      }
    }
    stage('maven install') {
        steps {
          withMaven(maven: 'Maven3') {
            sh 'mvn clean install'
        }
      }
    }
  }
}
