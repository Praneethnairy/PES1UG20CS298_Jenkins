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
                currentBuild.result = 'FAILURE' 
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
