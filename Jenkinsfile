#!groovy
pipeline {
    agent none
    tools {
      maven 'maven3'
      
    }
   stages {     
      stage('Compile') {
            steps {
                sh "mvn clean compile"
            }
        }
   }
}
