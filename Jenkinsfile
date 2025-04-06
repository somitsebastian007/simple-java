pipeline {
    agent any

    tools {
        maven 'Maven 3' // Make sure Maven is configured in Jenkins under Global Tool Configuration
        jdk 'Java 21'   // Also configure Java 17 there
    }

    stages {

        stage('Build with Maven') {
            steps {
                sh 'mvn clean package'
            }
        }

    }
}
