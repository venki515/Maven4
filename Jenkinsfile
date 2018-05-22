pipeline {
	agent any
	stages {
		stage ('Copiling Stage') {
			withMaven (maven : 'apache-maven-3.5.3') {
			sh 'mvn clean compile'
			}
		}
	}
}