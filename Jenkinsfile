#!groovy
pipeline {
    agent any 
    tools {
      maven 'maven3'
      
    }
   stages {     
      stage('Compile') {
            steps {
                bat "mvn clean compile"
            }
        }
        stage('Docker Build') {./mvnw package
          agent any
           steps {
             bat 'docker build -t mdp/spring-petclinic:latest .'
      }
    }
   }
}