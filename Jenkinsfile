pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
            browserstack(credentialsId: '982cb298-6b35-425a-abcc-a70671df986c'){
                sh "mvn clean"
                }
            }
        }
        stage('--test--') {
            steps {
                sh "mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }

    }
}