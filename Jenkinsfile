pipeline{
    agent any
	options {
        // This is required if you want to clean before build
        skipDefaultCheckout(true)
    }
    stages{
        stage('1-my name'){
            steps{
		    cleanWs()
                // We need to explicitly checkout from SCM here
                checkout scm
                echo "Building ${env.JOB_NAME}..."
                echo "My name is Abayomi"
                sh 'ps -ef'
            }   
        }
       
    }
}

