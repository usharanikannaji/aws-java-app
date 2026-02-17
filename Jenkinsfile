pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Deploy') {
            steps {
                sh 'java -jar target/aws-java-app-1.0-SNAPSHOT.jar'
            }
        }
    }
}

