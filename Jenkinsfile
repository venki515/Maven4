pipeline{
	agent any
	stages{
		stage('Compile stage'){
			steps{
				withMaven(maven : 'apache-maven-3.5.3')
					{
						sh 'mvn compile'
					}
				}
			}
		stage('Test stage'){
		steps{
				withMaven(maven : 'apache-maven-3')
				{
					sh 'mvn test'
				}
			}
		}
		stage('Deploy stage'){
			steps{
				withMaven(maven : 'apache-maven-3')
				{
					sh 'mvn deploy'
				}
			}
		}
	}
}