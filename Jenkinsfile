pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Example') {
            steps {
                echo ' Welcome to Jenkins declarative Pipe with Snipper Generator line Hello World '
                git branch: 'main', credentialsId: 'fa59e055-66c1-401c-abcc-9a5fb41924c9', url: 'https://github.com/srinivasivygit/jenkins.git'
            }
        }
    }
}
