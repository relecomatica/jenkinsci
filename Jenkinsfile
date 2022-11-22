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

def mostrarPoblacionNeta(Integer)
{
    def habitantes = 3223000 / 2
    println habitantes
}
