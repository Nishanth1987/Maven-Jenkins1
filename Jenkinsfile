pipeline {
	agent any

	stages {
		stage ('Compile Stage') {
			
			steps 
		{
				withMaven(maven : 'Maven') 
			{
				sh 'mvn clean compile'
				}
			}
		}
		
		stage ('Test Stage') {
			
			steps 
		{
				withMaven(maven : 'Maven') 
			{
				sh 'mvn test'
				}
			}
		}			
		
		stage ('Deployment Stage') {
			
			steps 
			{
				withMaven(maven : 'Maven') 
			{
				sh 'mvn deploy'
				}
			}
		}
	}
}
