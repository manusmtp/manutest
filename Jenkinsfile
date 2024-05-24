pipeline {
    agent any
    parameters{
      string(name: 'SERVERS', defaultValue: '192.0.2.0,192.0.2.1', description: 'Enter the IP addresses of the servers, separated by commas')
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
  }
} 

        
