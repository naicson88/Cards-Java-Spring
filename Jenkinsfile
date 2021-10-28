pipeline {
	agent any
	
	stages {
		stage ('Compile Stage'){
			steps{
				withMaven(maven: 'maven_3_5_0'){
					sh 'mvn clean compile'
<<<<<<< HEAD
					sh 'mvn -f yugioh-back/pom.xml clean install'
=======
					sh 'mvn -f yugioh-back/pom.xml'
					
>>>>>>> 109666adb5058f5622960f3408175c0ac085fbb8
				}
			}
			
		}
		
		stage ('Testing Stage'){
			steps{
				withMaven(maven: 'maven_3_5_0'){
					sh 'mvn test'
				}
			}
        }	
		stage ('Deployment Stage'){
			steps{
				withMaven(maven: 'maven_3_5_0'){
					sh 'mvn deploy'
				}
			}
			
		}
			
		}
	}
	
