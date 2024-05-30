pipeline{
   agent any
   stages{
        stage('ansible stage'){
            steps{
                script{
                    ansiblePlaybook(credentialsId: 'mcred', inventory: 'inventory.txt', playbook: 'play1.yml')
                }
            }
                 
        }
   }

}
