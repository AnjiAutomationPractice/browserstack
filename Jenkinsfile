pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {

                sh "mvn clean"

            }
        }
        stage('--test--') {
            steps {
                sh "mvn test -P parallel"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }

    }
}