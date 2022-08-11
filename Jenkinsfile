pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                retry(10) {
                    sh 'cat flakey-deploy'
                }

                timeout(time: 3, unit: 'SECONDS') {
                    sh 'cat flakey-deploy'
                }
            }
        }
    }
}