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
   }
}
