pipeline {
	agent any

	stages {
		stage ('Compile Stage') {
			
			steps 
		{
				withMaven(maven : 'Maven_3_8_6') 
			{
				sh 'mvn clean compile'
				}
			}
		}
		
		stage ('Test Stage') {
			
			steps 
		{
				withMaven(maven : 'Maven_3_8_6') 
			{
				sh 'mvn test'
				}
			}
		}			
		
		stage ('Deployment Stage') {
			
			steps 
			{
				withMaven(maven : 'Maven_3_8_6') 
			{
				sh 'mvn deploy'
				}
			}
		}
	}
}
