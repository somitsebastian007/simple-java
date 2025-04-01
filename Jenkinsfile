pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Replace with your GitHub repository URL
                git url: 'https://github.com/somitsebastian007/simple-java.git', branch: 'main'
            }
        }
        
        stage('Build') {
            steps {
                // Assuming you're using Maven - adjust if you're using Gradle or something else
                sh 'mvn clean package'
            }
        }
        
        // stage('Test') {
        //     steps {
        //         sh 'mvn test'
        //     }
        // }
        
        // stage('Deploy Locally') {
        //     steps {
        //         // Example: Copy the JAR to a local directory and run it
        //         sh '''
        //             cp target/*.jar /path/to/local/deployment/directory/
        //             # Kill any existing instance (optional)
        //             pkill -f 'java -jar' || true
        //             # Start the application in background
        //             nohup java -jar /path/to/local/deployment/directory/your-app.jar &
        //         '''
        //     }
        // }
    }
    
//     // post {
//     //     success {
//     //         echo 'Build and deployment completed successfully!'
//     //     }
//     //     failure {
//     //         echo 'Build or deployment failed!'
//     //     }
//     // }
 }