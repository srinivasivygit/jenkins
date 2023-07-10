pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Example') {
            steps {
			    // FIRST stage declarative pipeline stage-1
                echo ' Welcome to SECOND stage to Jenkins declarative Pipe with Snipper Generator line Hello World '
                git branch: 'main', credentialsId: 'fa59e055-66c1-401c-abcc-9a5fb41924c9', url: 'https://github.com/srinivasivygit/jenkins.git'
            }
        }
		stage('Test') { 
            steps {
                // SECONDS stage 
				echo ' Welcome SECOND stage to Jenkin Testing '

            }
        }
		
		stage('Deploy') { 
            steps {
                //  THIRD stage 
				echo ' Welcome THIRD stage to Jenkin  Deployment'
            }
        }
    }
}
