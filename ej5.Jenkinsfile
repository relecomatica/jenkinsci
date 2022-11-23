def TemActual = 12
def SumNum = 150 * 350
def NumPi = 
def BUILD_USER = "Jhon Montes"
pipeline {
    agent any 
    
    stages {
        stage("Comprobar fecha") {
            steps {
                script {
                    def dia = new Date().getDay()
                    def map=[
                        1:"Lunes",
                        2:"Martes",
                        3:"Miercoles",
                        4:"Jueves",
                        5:"Viernes",
                        6:"Sabado",
                        7:"Domingo",
                    ]  
                    println map[dia]
                    if ( map[dia] = 1 )
                    {
                    println map[dia] TemActual
                    }
                }
            }
        }
    }
}
