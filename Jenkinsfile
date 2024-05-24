pipeline {
    agent any
    parameters{
      string(name: 'SERVERS', defaultValue: '192.0.2.0,192.0.2.1', description: 'Enter the IP addresses of the servers, separated by commas')
      text(name: 'username', description:'Enter the username for the server')
      password(name: 'pass1', description: 'Enter password')
}
stages{
    stage('create the inventory '){
        steps{
        script{
            writeFile file: 'inventory.ini', text: """
                [webservers]
                ${params.SERVERS}
            """
        }
    }
    }
  

  stage('Run Ansible Playbook') {
            steps {
                // Run your Ansible playbook
                sh "sudo ansible-playbook -i inventory.ini play1.yml "
            }
        }
}
} 

        
