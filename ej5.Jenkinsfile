def TemActual = 12
def SumNum = 150 + 350
def NumPi = Math.PI
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
				    echo "Temperatura Actual: "
				    println TemActual
		                    break; 
	                    case 2: 
		                    println("Martes");
				    echo "Suma de dos numeros: "
				    println SumNum
		                    break; 
	                    case 3: 
		                    println("Miercoles");
				    echo "Numero PI: " 
				    println NumPi
		                    break; 
	                    case 4: 
		                    println("Jueves");
				    echo "Usuario que ejecuta el proceso: "
				    println BUILD_USER
		                    break; 
	                    case 5: 
		                    println("Viernes");
				    echo "Version Java"
				    ComprobamosVersionJava('Version Java')
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
def ComprobamosVersionJava(String a)
{
    sh "java --version"
    echo a
}

