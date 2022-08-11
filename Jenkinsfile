pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                retry(3) {
                    sh 'cat flakey-deploy'
                }

                timeout(time: 3, unit: 'MINUTES') {
                    sh 'cat flakey-deploy'
                }
            }
        }
    }
}