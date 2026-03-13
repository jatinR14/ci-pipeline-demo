pipeline {
    agent any

    stages {

        stage('Checkout_Code') {
            steps {
                git branch: 'main', url: 'https://github.com/jatinR14/ci-pipeline-demo.git'
            }
        }

        stage('Build_Project') {
            steps {
                bat '"C:\\apache-maven\\apache-maven-3.9.14\\bin\\mvn" clean install'
            }
        }

        stage('Run_Test') {
            steps {
                bat 'echo Running Tests'
            }
        }

        stage('Deploy_App') {
            steps {
                bat 'echo Deploying Application'
            }
        }

    }
}
