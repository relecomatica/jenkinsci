def hora = "new Date().format('HH')"
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

