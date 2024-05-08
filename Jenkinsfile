pipeline {
    agent any
    stages {
          stage('Docker login') {
                                        steps {
                                            withCredentials([usernamePassword(credentialsId: 'dockerL', Username: uname , Password: passw )]) {
                                                sh 'docker login -u $uname -p $passw' 
                                                }
                                           }
        
        }
    }

}
