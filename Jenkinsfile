pipeline {
    agent any 
    enviroment {
                NAME = "Dima"
                SURNAME = "Melnychuk"
                URL_NAME = "index.html"
            }
    stages {
        stage("Stage - 1") {
            steps {
                echo "HELLO ${NAME} ${SURNAME}"
                echo ${URL_NAME}
                timeout(time: 10, unit: 'SECONDS') {
                    sh "printenv"
                }
            }
        }
    }
}