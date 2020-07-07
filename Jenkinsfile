pipeline 
{
    agent any

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