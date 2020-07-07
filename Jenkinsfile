pipeline 
{
    agent any
    tools
    { 
        maven 'Maven 3.3.9' 
        jdk 'jdk8' 
    }

    stages 
    {
        stage ('Initialize') 
        {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
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