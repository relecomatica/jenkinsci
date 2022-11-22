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
                    def hora = "HH"
                    def dateTime1 = new Date().parse(hora)
                    def dateTime2 = new Date().parse(hora, "12")
                    println hora
                    if( "hora" > 12 )
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

