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
                    def now = new Date().format('HH')
                    def stringDate = "12"
                    def parsedDate= parse("HH", stringDate)
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

