pipeline {
	agent any
	stages {
		stage ('Copiling Stage') {
			steps {
			Maven (maven : 'apache-maven-3.5.3') {
			sh 'mvn clean compile'
			}
		}
	}
}
}