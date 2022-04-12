pipeline {
    agent any

    stages {
        stage('Checkout repo') {
            steps {
                git 'https://github.com/mostafabadry33/weather_app.git'
                
            }
        }
        stage('Build') { 
            steps { 
                sh 'make' 
            }
        }
        stage('Test'){
            steps {
                sh 'make check'
                junit 'reports/**/*.xml' 
            }
        }
        stage('Deploy') {
            steps {
                sh 'make publish'
            }
        }
    }
}
