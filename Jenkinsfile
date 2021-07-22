pipeline {
  agent any

  stages {
    stage('Build Test and Package') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}
