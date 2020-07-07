pipeline 
{
    agent any

    stages 
    {
        stage ('Initialize') 
        {
            steps {
                sh "mvn -version"
                sh "mvn clean install"
            }
        }

        stage('Build') 
        {
            steps 
            {
                echo 'building the app'
                script
                {
                    def test = 2 + 2 > 3 ? 'cool' : 'not cool'
                    echo test
                }
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