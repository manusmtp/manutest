pipeline {
    agent any
    environment{ 
              dockerL = credentials('dockerL')
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
