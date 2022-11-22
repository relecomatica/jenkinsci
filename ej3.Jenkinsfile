def top5Peliculas = "Gozilla,Superman,La liga de Justicia, El Señor de los Anillos, Destino Final"
def comidaFavorita = "Paella"
def signoZodiacal = "Cancer"
def PuestoActual = "Administrador de Sistemas"
def SalarioBruto = 900

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
                            mostrarSalarioNeto(1)
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

def mostrarSalarioNeto(Integer)
{

    def SalarioNeto = 30000 * 0.80
    println SalarioNeto
}
