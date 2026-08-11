pipeline
{
    agent any
    stages
    {
        stage('Compile')
        {
            steps
            {
                dir('src')
                {
                    bat 'javac hi.java'
                }
            }
        }
        stage('Run')
        {
            steps
            {
                dir('src')
                {
                    bat 'java hi'
                }
            }
        }
    }
    post
    {
        sucess
        {
            echo  'BUILD SUCCESSFUL'
        }
        failure
        {
            echo 'BUILDFAILED'
        }
    }
}