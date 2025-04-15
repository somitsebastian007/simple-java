pipeline {

    agent any

    tools{
        maven 'Maven 3'
        jdk 'Java 21'
    }

    stages{

        stage('Build with Maven')
        {
           steps{
            sh 'java --version'
            sh 'mvn --version'
            sh 'mvn clean package'
            sh 'java -jar target/hello-world-1.0-SNAPSHOT.jar'
           }
        }

    }


} 