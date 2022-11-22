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
                    Date now = new Date()
                    String stringDate = "10-03-2017"
                    Date parsedDate= Date.parse("dd-MM-yyyy", stringDate)
                    if(parsedDate > now)
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

