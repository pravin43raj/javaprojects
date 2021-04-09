pipeline{
  agent any
  stages {
    stage('Build jar file stage'){
      steps {
        withMaven(maven : 'maven3.6.3') {
          sh 'mvn clean install'
        }  
      }
    }
    stage('Build docker image stage'){
      steps {
        docker build . 
      }
    }
  }
}
