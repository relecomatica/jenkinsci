def numA = 100
def numB = 456
def BUILD_USER = "Jhon Montes"
def FechaAtual = new Date()
def TemActual = 12

pipeline {
    agent any 
    
    stages {
        stage("Comprobar fecha") {
            steps {
                script {
                    def dia = 1
                    def map=[
                        1:"Lunes",
                        2:"Martes",
                        3:"Miercoles",
                        4:"Jueves",
                    ]  
                    switch(dia) {            
	                    case 1: 
		                    println("Lunes");
				    echo "SUMA"
                        	    def Suma = numA + numB
                        	    println Suma
				    echo "RESTA"
                                    def Resta = numA - numB
                                    println Resta
				    echo "MULTIPLICACION"
				    def Multiplicacion = numA * numB
                                    println Multiplicacion
				    echo "DIVICION"
				    def Divicion = numA / numB
                                    println Divicion
		                    break; 
	                    case 2: 
		                    println("Martes");
				    echo "Usuario que ejecuta el proceso: "
				    println BUILD_USER
				    echo "Hora actual"
				    println FechaAtual
		                    break; 
	                    case 3: 
		                    println("Miercoles");
				    echo "El Pipeline se ejecuto correctamente." 
		                    break; 
	                    case 4: 
		                    println("Jueves");
                        	    echo "Temperatura Actual: "
				    println TemActual
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
