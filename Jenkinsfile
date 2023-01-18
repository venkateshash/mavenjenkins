pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                bat 'mvn clean'
            }
        }

        stage('Test') 
        {
            steps 
            {
                echo 'Test App'
            }
        }

        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploy App'
            }
        }
    }

    post
    {

    	always
    	{
    		
    		 archiveArtifacts artifacts:'**/*.jsp,**/*.war,**/*.xml',followSymlinks:false
    	
    	} 

    }
}
