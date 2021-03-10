pipeline{
  agent any
  stages {
    stage('Build stage'){
      steps {
        withMaven(maven : 'maven3.6.3') {
          sh 'mvn clean install'
        }  
      }
    }
  }
}
