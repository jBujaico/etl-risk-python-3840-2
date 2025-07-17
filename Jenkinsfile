pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'develop', url: 'https://github.com/jBujaico/etl-risk-python-3840-2.git'
            }
        }

        stage('Ejecutar ETL') {
            steps {
                sh 'python extract.py'
            }
        }
    }
}
