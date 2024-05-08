pipeline {
    agent any

    stages {
        stage('Example') {
            steps {
                withCredentials([string(credentialsId: 'dockerl', variable: 'DOCKERL')]) {
                    // Your code here, DOCKERL variable can be used which contains the secret text of 'dockerl' credential ID.
                    echo "The secret text is ${DOCKERL}"
                }
            }
        }
    }
}
