pipeline {
  agent {
   node { 
      label 'slave01'
     
   }
} 
 
  
stages{
  stage('Change dir') {
      steps {   
       
          sh 'pwd'
          sh 'ls'
          checkout scm
          sh 'ls'
          sh 'git --version'
          echo "Branch: ${env.BRANCH_NAME}"
          sh 'printenv'
          sh 'sudo yarn'
          sh 'sudo yarn build'
        
         
        

       } 
    } 
  } 
}    
 
