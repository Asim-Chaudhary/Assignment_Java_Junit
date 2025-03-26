pipeline 
{
    agent any

    tools {
            maven 'Maven 3.9.9'
    }

    stages 
    {
        stage('Build') 
        {
            steps 
                {
                    git branch : 'main', url: 'https://github.com/Asim-Chaudhary/Assignment_Java_Junit_Jenkins_Integration.git'
                    bat 'mvn clean compile'
                
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
}
