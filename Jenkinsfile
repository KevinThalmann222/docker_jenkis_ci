pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout des Codes aus dem Repository
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                // Ausführen des Python-Skripts
                sh 'python print_time.py'
            }
        }
        stage('Test') {
            steps {
                // Ausführen des Python-Skripts-Test
                sh 'python print_time_test.py'
            }
        }
    }
}
