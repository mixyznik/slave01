pipeline {
  agent {
   node { 
      label 'slave01'
     
   }
} 
 
  
stages{
  stage('Clone') {
      steps {   
       
          sh 'pwd'
          sh 'ls'
          checkout scm
          sh 'ls'
          sh 'git --version'
          echo "Branch: ${env.BRANCH_NAME}"
       } 
    } 
   stage('Change dir') {
      steps {   
        dir ('/var/www/workspace/proba_slave01_ssh_master') {
          sh 'pwd'
          sh 'ls'
          sh 'yarn'
          sh 'yarn build'
          sh 'whoami'
          sh 'sudo pm2 restart pencil'
          
          
          
         
        }

       } 
    } 

  } 

}    
 
