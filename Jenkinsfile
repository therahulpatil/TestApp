pipeline {
   agent any 
   tools {
        maven 'Maven3.9.6' 
    }
   
   stages {
       stage('SCM CheckOut'){
          steps {
            git 'https://github.com/therahulpatil/TestApp'
          }
          }
      stage('Compile-Package'){
         steps {
             sh "mvn -version"
            
              }
         }
   }
   post {
      always {
         cleanWs()
      }
   }
}
