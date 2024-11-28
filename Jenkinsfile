pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'java HelloWorld'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                echo 'Deployment successful!'
            }
        }
    }

    post {
        always {
            echo 'Post-build actions are running...'
        }
        success {
            echo 'Build succeeded!'
        }
        failure {
            echo 'Build failed. Check logs for details.'
        }
        unstable {
            echo 'Build marked as unstable.'
        }
        cleanup {
            echo 'Cleaning up workspace...'
            cleanWs()
        }
    }
}
