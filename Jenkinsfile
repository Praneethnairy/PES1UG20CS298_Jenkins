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
                catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
                    echo "Pipeline Failure"
                    sh "exit 1"
                }
            }
        }
        stage('Deploy') { 
            steps {
                sh 'exit 0' 
            }
        }
    }
    post{
    	failure{
    		echo 'Pipeline Failed'
    	}
    }
}
