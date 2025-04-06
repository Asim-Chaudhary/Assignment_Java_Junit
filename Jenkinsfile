pipeline 
{
    agent any

    tools {
            maven 'Maven_2'
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

    post 
    {
            always
            { emailext body: 'The Pipeline was successful.', subject: 'Pipeline Status', to: 'asimchaudhary1996@gmail.com' }
    }
}
    
