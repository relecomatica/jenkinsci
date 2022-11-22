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
                    def hora = new Date().format('HH')
                    println hora
                    if( 2 > 12 )
                    {
                        echo "Ejecutamos Proceso"
                    }
                    else
                    {
                        echo "No Ejecutamos Proceso"
                        println hora
                    }
                }
            }
        }
    }
}

