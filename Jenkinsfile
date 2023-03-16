pipeline {
   agent any
   tools {
     maven "maven3.9.0"
   }
   stages {
     stage('gitClone'){
       steps {
         git 'https://github.com/annkessy/software-visa.git'
       }
     }
     stage('mavenBuild'){
       steps {
         sh 'mvn clean package'
       }
     }
      stage('codequality'){
       steps{
         sh 'mvn sonar:sonar'
       }
   }
}
