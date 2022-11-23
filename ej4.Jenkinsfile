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
                    def str = new Date().format('HH')
                    int intHora = str as Integer
                    if ( intHora > 7 )
                    {
                        echo "Ejecutamos Proceso"
                        EjecutamosProceso(java)
                        
                    }
                    else
                    {
                        echo "No Ejecutamos Proceso"
                        println intHora
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
