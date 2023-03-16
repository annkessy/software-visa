pipeline {
   agent any
   stages {
     stage('gitClone'){
       steps {
         git 'https://github.com/Nixonsama/softwear-visa.git'
       }
     }
     stage('mavenBuild'){
       steps {
         sh 'mvn clean package'
       }
     }
   }
}
