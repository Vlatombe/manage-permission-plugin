pipeline {
  agent any

  stages {
    stage('Build Test and Package') {
      steps {
        sh 'mvn clean install -B -Dmaven.test.failure.ignore=true -Dspotbugs.failOnError=false'
        junit '**/*-report/*.xml'
      }
    }
  }
}
