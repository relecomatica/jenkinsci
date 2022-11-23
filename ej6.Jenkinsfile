pipeline {
    agent any 
    
    stages {
        stage("Comprobar hora") {
            steps {
                script {
                    def str = new Date().format('HH')
                    int intHora = 9
		    if ( intHora <= 10 )
		    {
		    	EjecutamosComandoDos('ComandoDos')
		    }
		    else if ( intHora >= 11 && intHora <= 15 )
		    {
		    	ComprobamosVersionGit('Version Git')
		    }
		    else if ( intHora >= 16 && intHora <= 22 )
		    {
		    	HoraSistema('Hora')
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
def HoraSistema(String a)
{
    sh "time"
    echo a
}
