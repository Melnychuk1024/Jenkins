pipeline {
    agent any 
    stages {
        stage("Stage - 1") {
           environment {
                NAME = "Dima"
                SURNAME = "Melnychuk"
                URL_NAME = "index.html"
            }
            steps {
                 echo "HELLO ${NAME} ${SURNAME}"
                 sh "cat ${URL_NAME}"
                timeout(time: 10, unit: 'SECONDS') {
                    sh "printenv"
                }
            }
        }
    }
}