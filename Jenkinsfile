pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'exit 0'
            }
        }
        stage('Test') { 
            steps {
                sh 'exit 0'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'exit 0' 
            }
        }
    }
    post{
        success{
            echo 'Pipeline Success'
        }
    	failure{
    		echo 'Pipeline Failed'
    	}
    }
}
