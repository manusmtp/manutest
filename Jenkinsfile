pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Add your build steps here
                sh 'echo "Building..."'
            }
        }
        stage('Test') {
            steps {
                // Add your test steps here
                sh 'echo "Testing..."'
            }
        }
        stage('Deploy') {
            steps {
                // Add your deployment steps here
                sh 'echo "Deploying..."'
            }
        }
    }
    
    post {
        success {
            // Actions to take if the pipeline succeeds
            echo 'Pipeline succeeded!'
        }
        failure {
            // Actions to take if the pipeline fails
            echo 'Pipeline failed!'
        }
        always {
            // Actions to take always, regardless of success or failure
            echo 'Pipeline completed!'
        }
    }
}

