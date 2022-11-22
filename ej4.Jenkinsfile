def hora = new Date().format('HH')
pipeline
{
    agent any
    stages
    {
        stage("Prebuild")
        {
            steps
            {
                
                script
                {
                    if( hora < 12 )
                        {
                            EjecutamosProceso('java')
                        }
                        else
                        {
                            echo "No ejecutamos el proceso"
                            println hora
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
