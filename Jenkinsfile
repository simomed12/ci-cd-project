pipeline {
    agent any 
    tools {
        jdk 'Java17'
        maven 'Maven3'
    }
    stages {
        
        stage('Cleanup Workspace') {
            steps {
                cleanWs()
            }
        }
    
        stage('Checkout from SCM') {
            steps {
                git branch: 'main', 
                    credentialsId: 'github', 
                    url: 'https://github.com/simomed12/ci-cd-project.git'
            }
        }

    }
}

