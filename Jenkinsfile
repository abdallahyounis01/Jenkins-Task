pipeline {
     agent any
      parameters {
        booleanParam(name:'Bool-Para', defaultValue: true, description:'this paramater help you to know project name')
    }
   
    stages {
        stage('Check') {
            steps {
                echo "Checking Your Code"
               
            }
        }

        stage('Test') {
            when {
                expression{
                    params.Bool-Param == true 
                }
            }
            steps {
                echo "Testing Your App" 
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
