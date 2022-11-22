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
                            def user = cause.userId
                            echo "started by ${user}"
                            echo "Ejecutamos Proceso"
                            EjecutamosProceso()
                           
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

