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
                sh "mvn test -f maventestjenkins"                
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package -f maventestjenkins"                
 
            }
        }
    }
}
