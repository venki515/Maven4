pipeline{
	agent any
	tools{
		maven 'apache-maven-3.5.3'
		}
	stages{
		stage('Initialization'){
			steps{
				bat '''
					echo "PATH=${PATH}"
					echo "M2_HOME=${M2_HOME}"
					'''
				}
			}
		stage('Compiliation'){
			steps{
				bat 'mvn clean compile'
			}
			
		}
		stage('Package'){
			steps{
				bat 'mvn package'
			}
		}
		
	}
}
		