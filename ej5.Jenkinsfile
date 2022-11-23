def TemActual = 12
def SumNum = 150 * 350
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
                    switch(dia) {            
	                    case 1: 
		                    println("The value of a is One"); 
		                    break; 
	                    case 2: 
		                    println("The value of a is Two"); 
		                    break; 
	                    case 3: 
		                    println("The value of a is Three"); 
		                    break; 
	                    case 4: 
		                    println("The value of a is Four"); 
		                    break; 
	                    default: 
		                    println("The value is unknown"); 
		                    break; 
                    }

                }
            }
        }
    }
}
