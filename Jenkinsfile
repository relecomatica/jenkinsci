def temActual = 10
def canHabitantes = 3223

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

def mostrarPoblacionNeta(Integer a)
{
    def Poblacion = canHabitantes/2
    return a
}
