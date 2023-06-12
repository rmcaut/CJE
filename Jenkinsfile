pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building the project..."'
            }
        }
        
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'echo "Deploying the application..."'
            }
        }
    }
    
    post {
        always {
            echo 'This will always execute'
        }
        
        success {
            echo 'This will only execute on success'
        }
        
        failure {
            echo 'This will only execute on failure'
        }
    }
}
