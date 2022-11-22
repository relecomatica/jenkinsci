def top5Peliculas = "1-Gozilla, 2-Superman, 3-La liga de Justicia, 4-El Señor de los Anillos, 5-Destino Final"
def comidaFavorita = "Paella"
def signoZodiacal = "Cancer"
def PuestoActual = "Administrador de Sistemas"
def SalarioBruto = 33000

pipeline {
    agent any

    stages {
        stage('Top 5 Peliculas Favoritas') {
            steps {
                println top5Peliculas
            }
        }
        stage('Comida Favorita') {
            steps {
                println comidaFavorita
            }
        }
        stage('Signo Zodiacal') {
            steps {
                println signoZodiacal
            }
        }
        stage('Puesto Actual') {
            steps {
                println PuestoActual
            }
        }
        stage('Salario Bruto') {
            steps {
                println SalarioBruto
            }
        }
        stage("Prebuild")
            {
                steps
                {
                    script
                    {
                        if( SalarioBruto > 1000 )
                        {
                            mostrarSalarioNeto(SalarioBruto)
                        }
                        else
                        {
                            echo "Salario Neto"
                            println SalarioBruto
                        }
                    }
                }
            }
    }
}

def mostrarSalarioNeto(Integer SalarioBruto)
{
    def SalarioNeto = SalarioBruto * 0.80
    println SalarioNeto
}
