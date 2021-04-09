pipeline {
  agent any
  stages {
    stage('Build stage') {
      steps {
        withMaven(maven : 'maven3.6.3') {
          sh 'mvn clean install'
        }  
      }
    }
    stage('Build docker image') {
      steps {
        sh 'cd spring-boot-hello-world-example'
        sh 'docker build .'
      }  
    }  
  }
}  
