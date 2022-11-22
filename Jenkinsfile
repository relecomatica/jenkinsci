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
                        mostrarPoblacionNeta('poblacion neta')
                    }
                }
            }
    }
}

def mostrarPoblacionNeta(String a)
{
    bash "canHabitantes / 2"
    echo a
}
