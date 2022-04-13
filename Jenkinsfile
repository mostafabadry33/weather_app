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
        sh 'echo " building complate "'
      }
    }

    stage('Test') {
      steps {
        sh 'echo " testing complate "'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo " deploying complate "'
      }
    }

  }
}