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
        stage('Docker Build') {
          agent any
           steps {
             bat 'docker build -t mdngphg411/spring-petclinic:latest .'
      }
    }
   }
}
