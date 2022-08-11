pipeline {
    agent none
    stages {
        stage('Build...') {
            agent {
                docker {image 'hello-world:latest'}
            }
            steps {
                 sh 'sudo docker run hello-world'
            }
        }
    }
}