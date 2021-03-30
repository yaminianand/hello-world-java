pipeline {
   agent any

   stages {
      stage('Checkout') {
         steps {
            git 'https://github.com/AnjuMeleth/hello-world-java.git'
         }
      }
      stage('Build'){
        steps {
            sh 'sudo docker build . -t yaminianand/mytomcat1'
            sh 'sudo docker push yaminianand/mytomcat1'
        }
      }
   }
}
