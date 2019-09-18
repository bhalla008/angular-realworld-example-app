pipeline{
  agent any
  tools {nodejs "node"}
  stages{
    stage ('checkout'){
      steps{
        checkout scm
      }
    }
    stage ('install modules'){
      steps{
        
        sh   'npm install -g @angular/cli'
        sh  'npm install --verbose -d'
      } 
	  }
    stage ('build'){
      steps{
         sh 'npm run build'
          }
    } 
    
    stage ('deploy'){
      steps{
         sh 'pm2 restart all'
          }
    } 
    }

 }

