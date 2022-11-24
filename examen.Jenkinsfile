def numA = 100
def numB = 456
def TemActual = 12
def NumPi = Math.PI
def BUILD_USER = "Jhon Montes"
pipeline {
    agent any 
    
    stages {
        stage("Comprobar fecha") {
            steps {
                script {
                    def dia = Lunes
                    def map=[
                        1:"Lunes",
                        2:"Martes",
                        3:"Miercoles",
                        4:"Jueves",
                    ]  
                    switch(dia) {            
	                    case 1: 
		                    println("Lunes");
                        def Suma = numA + numB
                        println Suma
                        def Resta = numA - numB
                        println Resta
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
                        echo "Temperatura Actual: "
				                println TemActual
				                echo "Usuario que ejecuta el proceso: "
				                println BUILD_USER
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
def ComprobamosVersionJava(String a)
{
    sh "java --version"
    echo a
}
