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
                    int num = str as Integer
                    if ( num > 12 )
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

