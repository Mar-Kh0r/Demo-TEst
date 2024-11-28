pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Compile the Java file on Windows
                bat 'javac HelloWorld.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Run the compiled Java program on Windows
                bat 'java HelloWorld'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Placeholder for deployment logic
                echo 'Deployment successful!'
            }
        }
    }
}
