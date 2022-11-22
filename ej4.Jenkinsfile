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
                    if( hora < 12 )
                        {
                            echo "Ejecutamos proceso"    
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

