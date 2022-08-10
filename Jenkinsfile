pipeline {
    agent any
    stages {
        
        stage('Test') {
            docker { image 'node:16.13.1-alpine' }
            steps {
                echo "Test"
                sh 'node --version'
            }
        }
    }
}
