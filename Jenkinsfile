pipeline {
  agent any
  environment {
    dockerImage=''
    registry='pravinkumbhar/repo1'
  }
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
            dockerImage = docker.build ./spring-boot-hello-world-example/ registry
      }  
    }  
  }
}  
