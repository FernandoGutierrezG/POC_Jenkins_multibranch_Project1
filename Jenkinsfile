pipeline 
{
    agent any

    tools {
        maven "3.6.0" // You need to add a maven with name "3.6.0" in the Global Tools Configuration page
    }
    stages 
    {

        stage('Build') 
        {
            steps 
            {
                echo 'building the app'
                sh 'mvn -version'
                sh 'mvn clean install'
                echo 'app builded'
            }
        }

        stage('test') 
        {
            steps 
            {
                echo 'testing the app'
            }
        }

        stage('deploy') 
        {
            steps 
            {
                echo 'deploying the app'
            }
        }
    }
}