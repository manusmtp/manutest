pipeline {
    agent any

    stages {
        stage('Docker login') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'dockerl', usernameVariable: 'DOCKER_USER', passwordVariable: 'DOCKER_PASSWORD')]) {
                    sh "docker login -u ${DOCKER_USER} -p ${DOCKER_PASSWORD} manusmtp"
                }
            }
        }
        // Additional stages here...
    }
}
