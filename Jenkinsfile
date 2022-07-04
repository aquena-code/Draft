pipeline{
    agent any
    environment {
        service_name = "Reporting Service"
    }
    stages{
        stage ("Step 1"){
            steps {
                echo "${service_name}"
                echo "This is the step 1"
            }
        }
    }
    
    post {
        always {
            echo "Always Run after ${service_name}"
        }
        success {
            echo "The ${service_name} was executed successfully !!!" 
        }
        failure {
            echo "Failed execution......"
        }
    }
    
}