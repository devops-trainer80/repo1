pipeline {
    agent any
    
    stages{
        stage('build'){
             steps {
               echo ' Buidling the Applicaion'
            }
        }
    stage('test'){
        when{
            branch 'production'
        }
            steps{
        echo 'Testing apllication successfully'        
            }
        
        }
    }
    post{
        always{
            echo 'willexecute the pipeline again'
        }
        
        success{
            'successfully executed the steps'
        }
    }
}
