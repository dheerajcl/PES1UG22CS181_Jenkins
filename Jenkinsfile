pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'moan -C main'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh './main/hello_exec'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                echo 'Deployment completed (simulated).'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}       