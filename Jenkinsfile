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
        sh 'docker build -t spring-boot-hello-world-example ./spring-boot-hello-world-example/'
        sh 'docker image tag spring-boot-hello-world-example spring-boot-hello-world-example:1.0.0'
        sh 'docker build -t spring-boot-project ./spring-boot-project/'
        sh 'docker image tag spring-boot-project spring-boot-project:1.0.0'
      }  
    }  
  }
}  
