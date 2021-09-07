pipeline {
agent any 
	stages {
		stage('checkoutscm') {
			steps{
			git credentialsId: 'github-password', url: 'https://github.com/rojabm1998/Javawebapp.git'
			}
		}
		stage('maven build') {
			steps{
				//cd Javawebapp
				sh 'mvn clean install'
			}
		}
		
	}
}
