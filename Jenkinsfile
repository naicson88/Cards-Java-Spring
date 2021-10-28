pipeline {
	agent {
		docker{
			image "maven:3.8.3-jdk-11"
			label "docker"
		}
	}
	
		stages {
			stage ('Compile Stage'){
				steps{
					
						sh 'mvn clean compile'
						sh 'mvn clean install'
					
				}
				
			}
			
			stage ('Testing Stage'){
				steps{
					withMaven(maven: 'Maven3.8.3'){
						sh 'mvn test'
					}
				}
			}	
			
				
		}
		
		post {
				always{
					cleanWs
				}
			}
	}
