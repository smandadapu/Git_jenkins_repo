pipeline {
    /* insert Declarative Pipeline here
     build , test and deploy
	 build test and deploy
	*/
	
	agent { label 'Jenkinsmaster' }
	
	 tools {
        maven 'maven-3.5'
        jdk 'jdk1.8'
    }
	 stages { 
        stage('scm') {
            steps {
                echo 'chekout step'
				git 'https://github.com/smandadapu/Jenkins-maven-axa-dev.git'
				
            }
			}
		stage('build') {
            steps {
               bat "mvn clean install"
            }
        }
    
	
}

}
