pipeline {
    agent any
         stages{
            stage('1stage'){
                input{
                    message "this is form"
                 parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                }
            }
        steps {
                echo "Hello, ${PERSON}, nice to meet you."
            }
        }
    }
        
}
        
