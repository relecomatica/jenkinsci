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
                    if( hora > 12 )
                        {
                            echo "${GIT_AUTHOR_NAME}"
                            echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
                            echo "Ejecutamos Proceso"
                            EjecutamosProceso(java)
                        }
                        else
                        {
                            echo "No ejecutamos el proceso"
                        }
                }
                
            }
        }
    }
}
def EjecutamosProceso(String a)
{
    sh "java --version"
    echo a
}

