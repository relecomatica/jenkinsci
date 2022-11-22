def temActual = 10
def canHabitantes = 3223000

pipeline {
    agent any

    stages {
        stage('Temperatura Madrid') {
            steps {
                println temActual
            }
        }
        stage('Habitantes Madrid') {
            steps {
                println canHabitantes
            }
        }
        stage("Prebuild")
            {
                steps
                {
                    script
                    {
                        mostrarPoblacionNeta(1)
                    }
                }
            }
    }
}

def mostrarPoblacionNeta(Integer 1)
{
    def Poblacion = 3223000/2
    return 1
}
