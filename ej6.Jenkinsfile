pipeline {
    agent any 
    
    stages {
        stage("Comprobar hora") {
            steps {
                script {
                    def str = new Date().format('HH')
                    int intHora = str as Integer

                    switch(intHora) {            
	                    case 1:
                        while(intHora=<10) {
                        EjecutamosComandoDos('ComandoDos')
                        }
				                echo "Temperatura Actual: "
				                println TemActual
		                    break; 
	                    case 2: 
                        while(intHora>=11 && intHora=<15) {
                        ComprobamosVersionGit('Version Git')
                        }
		                    break; 
	                    case 3: 
		                    println("Miercoles");
				                echo "Numero PI: " 
				                println NumPi
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
def ComprobamosVersionGit(String a)
{
    sh "git --version"
    echo a
}
def EjecutamosComandoDos(String a)
{
    sh "ifconfig"
    echo a
}

