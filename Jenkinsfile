pipeline {
    agent any

    parameters {
        choice(name: 'PLATFORM_FILTER', choices: ['all', 'linux', 'windows', 'mac'], description: 'Run on specific platform')
    } 

stages{
    stage('var output'){
            steps {
                echo "choice chosed by user :: ${params.PLATFORM_FILTER}"
            }
    }
} 
}
        
