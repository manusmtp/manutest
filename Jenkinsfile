pipeline {
    agent any
    environment{ 
              example_creds = credentials('dockerL')
    }
    stages {
        stage('Docker login') {
            steps {
                
                    sh('docker login -u $dockerL_USR -p $dockerL_PSW')
            }
        }
        // Additional stages here...
    }
}
