pipeline {
    agent any 
    stages {
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
        stage('Finish) {
	    steps{
	        echo 'FINISH'
             }
    }
}
