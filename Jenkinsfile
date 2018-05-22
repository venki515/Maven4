pipeline{
	agent any
	tools{
		maven 'apache-maven-3.5.3'
		}
	stages{
		stage ('Initialization') {
			steps{
				sh '''
					echo "PATH = ${PATH}"
					echo "M2_HOME = ${M2_HOME}"
					'''

			}
		stage ('Building Maven') {
			steps{
			sh 'mvn -Dmaven.test.fail.ignore=true clean build'
			}
		}
		}
	}
	}