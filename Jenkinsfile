pipeline {
    agent slave-1

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/nazishanwar1/maven-practice.git'
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

