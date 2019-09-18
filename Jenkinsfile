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
         sh 'npm start --host 0.0.0.0'
          }
    } 
    }

 }

