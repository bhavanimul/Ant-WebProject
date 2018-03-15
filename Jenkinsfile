#! groovy
node{
 stage('Source'){
     git 'https://github.com/bhavanimul/Ant-WebProject.git'
 }
 
 stage('Build'){
    
    bat "ant -f build-mt.xml" 
 }
 stage('Send Email'){
     mail bcc: 'bhavani.mul@gmail.com', body: 'Buils is done', cc: '', from: '', replyTo: '', subject: 'Build Status', to: 'bhavani.mul@gmail.com'
 }
 /*stage('Archive'){
  archiveArtifacts '/Users/bhaskarreddyl/.jenkins/workspace/Pipeline-Project-Ant-Web/dist/SampleAntProject.war'
 }*/
}
