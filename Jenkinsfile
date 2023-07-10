pipeline {
    agent any
    // Set the environment variable APP_PORT=9090
    environment{
        APP_PORT='9090'
    }
    stages {
        stage('Build') {
            steps {
               sh ' mvn -B package -DskiTests '
            }
        }
        stage('Unit Test') {
            steps {
                 sh 'mvn -B test'
            }
        }
    }
}
