pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat '"C:\\Program Files\\apache-maven-3.9.16\\bin\\mvn.cmd" clean package'
            }
        }

    }
}