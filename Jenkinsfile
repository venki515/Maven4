pipeline{
	agent any
	tools{
		maven 'apache-maven-3.5.3'
		}
	stages{
		stage('Initialization'){
			steps{
				bat '''
					echo "PATH = ${PATH}"
					echo "M2_HOME = ${M2_HOME}"
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
		stage('Deploy'){
			steps{
				bat'xcopy C:\Users\venkatesh\.jenkins\workspace\NewPipe\target\JenkinsWar.war C:\Users\venkatesh\Desktop\Jenkin &Tomcat\Tomcat\apache-tomcat-8.5.30\webapps'
			}
		}
	}
}
		