pipeline {
  agent any
  stages {
    stage('Inicio') {
      steps {
        echo 'Hola desde Stage Inicio'
      }
    }

    stage('Test2') {
      post {
        always {
          sh 'docker container stop app'
        }

      }
      steps {
        echo 'Hola desde stage 2'
      }
    }

  }
}