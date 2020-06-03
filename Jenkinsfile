pipeline {
   
   agent any
   
      tools {
        maven 'maven3.6.3'
        jdk 'jdk8'
        terraform 'terraform'

    	}
   stages {
   
      stage('version check') {
         steps {
             bat 'terraform --version'
             echo 'Hello World'
         }
      }
      
      stage('terraform initialize') {
        steps {
            bat 'terraform init'
            }
           }
           
      stage('plan') {
          steps {
              bat 'terraform plan'
              }
           }
     
   }
}
