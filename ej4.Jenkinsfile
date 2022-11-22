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
                    now = new Date().format('HH')
                    stringDate = "12"
                    parsedDate= Date.parse("HH", stringDate)
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

