pipeline {
    agent any
    stages {
        stage('Build...') {
            steps {
                echo "Deploy..."
            }
        }
        stage('Test...') {
            steps {
                echo "Test..."
            }
        }
        stage('Deploy')  {
             agent {
                docker {image 'hello-world:latest'}
            }
            steps {
                 sh 'sudo docker run hello-world'
            }
        }
    }
}