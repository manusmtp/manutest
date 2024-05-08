pipeline {
    agent any
    stages {
          stage('Docker login') {
                                        steps {
                                            withCredentials([file(credentialsId: 'dockerL', variable: uname)]) {
                                                sh ''
                                                }
                                           }
        
        }
    }

}
