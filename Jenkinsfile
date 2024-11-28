pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Compile the Java file
                sh 'javac HelloWorld.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Run the Java program and capture its output
                sh 'java HelloWorld'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Simulating deployment (customize as needed)
                echo 'Deployment successful!'
            }
        }
    }
}
