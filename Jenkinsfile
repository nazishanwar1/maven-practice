pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/nazishanwar1/maven-practice.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Run') {
            steps {
                sh 'java -jar target/maven-practice-1.0-SNAPSHOT.jar'
            }
        }
    }
}

