pipeline {
     agent any
  
    stages {
        stage('Build') {
            steps {
                echo "Checking Your Code"
            }
        }

        stage('Test') {
            when {
                expression{
                    params.BoolParam == true 
                }
            }
            steps {
                echo "Testing Your Code" 
            }
        }
        
        stage('Deployment') {  
            steps {
                echo "Your Code Is Deploying"
                echo "This Build Number $BUILD_NUMBER"
            }
        }    
    }

}
