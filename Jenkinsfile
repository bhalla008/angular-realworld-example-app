pipeline{
  agent any
  
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
    stage ('test'){
      steps{
         sh 'npm -vesrion'
          }
    } 
    }

 }

