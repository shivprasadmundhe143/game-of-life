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
		
		stage ('continous deploy') {
			steps {  
				sh 'cp /root/.jenkins/workspace/game-of-life/gameoflife-web/target/gameoflife.war /mnt/apache-tomcat-9.0.71/webapps'
				}
				}
				
		stage ('continous Deliver on QA') {
			steps {
				sh 'scp /root/.jenkins/workspace/game-of-life/gameoflife-web/target/gameoflife.war ansible@172.31.95.132://mnt/apache-tomcat-9.0.71/webapps'
				}
				}
				}
				}

		
