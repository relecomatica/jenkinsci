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
                    def Hora = new Date().format('HH')
                    def intHora = 'Hora' as int
                    if( intHora > 12)
                    {
                        echo "Ejecutamos Proceso"
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

