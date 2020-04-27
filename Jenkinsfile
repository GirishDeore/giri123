pipeline {
   agent any
   environment{ 
    PATH = "/opt/maven3/bin:$PATH"
   }
  
   stages {
      stage('git') {
         steps {
            git credentialsId: 'github', url: 'https://github.com/GirishDeore/giri123.git'
         }
      }
          stage('maven build') {
         steps {
            sh "mvn clean package"
         }
      }

   }
}
