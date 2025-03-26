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
                    git branch : 'main', url: 'https://github.com/Asim-Chaudhary/Assignment_Java_Junit.git'
                    bat 'mvn clean compile'
                
                }

        }

        stage('Test') 
        {
            steps 
                {
                bat 'mvn test'
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
