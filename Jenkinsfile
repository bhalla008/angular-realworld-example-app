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
    stage('yarn install') {
    steps{
        sh 'npm install -g yarn'
        sh 'yarn install'
    }
    }
    stage ('build'){
      steps{
         sh 'npm run build'
          }
    } 
    
    stage ('deploy'){
      steps{
         sh 'npm start'
          }
    } 
    }

 }

