def COLOR_MAP = [
    'SUCCESS': 'good', 
    'FAILURE': 'danger',
]

pipeline {

  agent any
 
  stages {
	stage('Publish to Exchange') {
         steps {
		   bat 'mvn -s C:/Users/rahulallam/.m2/settings.xml -X clean deploy'
		 }
		 }
    stage('Deploy to RTF') {
         steps {
		   bat 'mvn -s C:/Users/rahulallam/.m2/settings.xml -X clean deploy -DmuleDeploy'
		 }
		 }
	
   }
   
}