def comidaFavorita = Paella
def signoZodiacal = Cancer
def PuestoActual = Administrador de Sistemas
def SalarioBruto = 30000

pipeline {
    agent any

    stages {
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
                        mostrarSalarioNeto(1)
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
