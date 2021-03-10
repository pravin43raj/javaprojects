pipeline{
  agent any
  stages {
    stage('Build stage'){
      steps {
        withMaven(maven : '') {
          sh 'mvn clean install'
        }  
      }
    }
  }
}
