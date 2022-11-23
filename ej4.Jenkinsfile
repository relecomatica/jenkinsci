def BUILD_USER = "Jhon Montes"
def BUILD_USER_ID = 3680

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
                        echo "Version Java"
                        EjecutamosProceso('java version')
                        echo "Usuario que ejecuta el Proceso"
                        echo "$BUILD_USER"
                        echo "ID del Usuario que ejecuta el Proceso"
                        echo "$BUILD_USER_ID"
                        
                        
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
