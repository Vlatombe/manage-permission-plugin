pipeline {
  agent any

  stages {
    stage('Build Test and Package') {
      steps {
        sh 'mvn clean verify -B -Dmaven.test.failure.ignore=true -Dspotbugs.failOnError=false'
        junit '**/*-report/*.xml'
      }
    }
  }
}
