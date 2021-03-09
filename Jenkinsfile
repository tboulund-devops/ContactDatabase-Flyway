pipeline {
    agent any
    stages {
        stage("Deliver database") {
            steps {
                sh "docker-compose up app-database -d"
                sh "docker-compose up flyway"
            }
        }
    }
}