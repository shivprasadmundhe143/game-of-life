pipeline {
    agent any
	
	stages {
		stage ('continous download') {
			steps {
				git 'https://github.com/shivprasadmundhe143/game-of-life.git'
				}
				}
				
		stage ('continous build') {
			steps {
				sh 'mvn package'
				}
				}
			}
			}
		
