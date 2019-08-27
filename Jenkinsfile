pipeline {
    agent any 
    stages {
        stage('Starting') {
	    steps {
	    	echo 'Starting ......'
	    }	
	}
	stage('clone git repo') { 
            steps {
                sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"                
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package"                
             }
        }
    }
}
