pipeline {
  agent {
   node { 
      label 'slave01'
     
   }
} 
 
  
stages{
  stage('Change dir') {
      steps {   
        dir ('/var/www') {
          sh 'pwd'
          sh 'ls'
          sh 'git --version'
        
         
        }

       } 
    } 
  } 
}    
 
