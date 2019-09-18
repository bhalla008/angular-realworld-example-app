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
        sh '''
          npm install --verbose -d 
          npm install -g @angular/cli@6.0.8
	  npm -version
	'''
	}
    }

 }
}
