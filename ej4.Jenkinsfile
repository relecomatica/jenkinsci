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
                    def varHora = hora
                    if( varHora > 12 )
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

