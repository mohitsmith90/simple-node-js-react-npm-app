pipeline {
    agent {
        docker {
            image 'node:lts-buster-slim' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'sudo chown -R 990:987 "/.npm"' 
            }
             steps {
                sh 'npm install' 
            }
        }
    }
}
