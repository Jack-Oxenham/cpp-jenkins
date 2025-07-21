pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the C++ project...'
                sh 'make'
            }
        }

        stage('Run') {
            steps {
                echo 'Running the program...'
                sh './hello'
            }
        }
    }
}
