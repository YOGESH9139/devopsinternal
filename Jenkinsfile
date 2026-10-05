pipeline {
    agent any
    stages {
        stage ('Checkout') {
            steps {
                echo 'Checking application....'
                checkout scm
            }
        }
        stage ('Build') {
            steps {
                echo 'Building application...'
                bat '''
                    if not exist index.html /b 1
                '''
                echo 'All required files exist'
            }
        }
        stage ('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage ('Complete') {
            steps {
                echo 'Done'
            }
        }
        
    }
}