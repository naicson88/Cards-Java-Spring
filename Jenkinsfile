pipeline {
	agent {
		docker{
			image "maven:3.8.3-jdk-11"
			
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
					
						sh 'mvn test'
					
				}
			}	
			
				
		}

		
	}
