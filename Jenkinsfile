pipeline {
 agent { 
    node { label 'maven' }         
 }     
  
 //environment {
  //constants = load 'constants.groovy'
  //giturl = "${constants.giturl}"
// }
stages {
 
stage('git clone') {   
steps {
 
script {
 //def scmUrl = scm.getUserRemoteConfigs()[0].getUrl()
  //def constants = load 'constants.groovy'
  //def giturl = constants.giturl
  sh "echo ${env.GIT_URL}"
}
 // git url: "${env.giturl}"
 //}
  //git url: "${giturl}"
 //git url: 'https://github.com/shweta9651/java-junit-sample.git'
// git url: 'https://github.com/miguno/java-docker-build-tutorial.git'  

}
}  

stage('compile source code') {
     steps {
         sh 'mvn clean install'
   
     }
  }
    
 }
}   
 
