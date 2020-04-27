pipeline {
   agent any
   environment{ 
    PATH = "/home/sunbeam/Desktop/new_jenkins/my-app:$PATH"
   }
  
   stages {
      stage('git') {
         steps {
            git credentialsId: 'github', url: 'https://github.com/GirishDeore/giri123.git'
         }
      }
          stage('maven build') {
         steps {
            sh 'echo mvn clean package'
         }
      }

   }
}
