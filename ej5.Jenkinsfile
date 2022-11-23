import java.lang.System

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
		                    println("Lunes"); 
		                    break; 
	                    case 2: 
		                    println("Martes"); 
		                    break; 
	                    case 3: 
		                    println("Miercoles");
				    System.out.println(Math.PI);
		                    break; 
	                    case 4: 
		                    println("Jueves"); 
		                    break; 
	                    case 5: 
		                    println("Viernes"); 
		                    break; 
	                    case 6: 
		                    println("Sabado"); 
		                    break; 
	                    case 7: 
		                    println("Domingo"); 
		                    break; 				    
	                    default: 
		                    println("Valor desconocido"); 
		                    break; 
                    }

                }
            }
        }
    }
}
