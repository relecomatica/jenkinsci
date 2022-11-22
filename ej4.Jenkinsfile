pipeline
{
    agent any
    stages
    {
        stage("Ejecutar Proceso despues de las 12")
        {
            steps
            {
                
                script
                {
                    def hora = new Date().format('HH')
                    println hora
                    echo "${env.GIT_AUTHOR_NAME}"
                    echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
                    echo "Ejecutamos Proceso"
                   
                }
                
            }
        }
    }
}
