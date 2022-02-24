pipeline {
    agent any 
    tools {

        nodejs 'node-11.0.0'

    }
    options {

        timeout (time: 2, unit: 'MINUTES')

    }

    stages {
        stage('Install Dependecies') { 
            steps {
                sh 'npm i'
            }
        }
        stage('Run Tests') { 
            steps {
                sh 'npm run test'
            }
        }
    }
}