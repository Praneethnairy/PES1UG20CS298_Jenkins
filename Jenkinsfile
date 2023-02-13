pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'build'
            }
        }
        stage('Test') { 
            steps {
                echo 'test' 
            }
        }
        stage('Deploy') { 
            steps {
                echo 'deploy' 
            }
        }
    }
    post{
    	failure{
    		echo 'Pipeline Failed'
    	}
    }
}
