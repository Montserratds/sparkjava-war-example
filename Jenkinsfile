
pipeline {
  agent {label 'Díaz0'}
  stages {
    stage('Build') {
      steps {
        sh '''
        echo "Prueba shell"
        pwd
        mvn clean install
        '''
            }
    }
    stage('Test') {
      steps {
        echo "Do something"
      }
    }
    stage('Deploy') {
      steps {
        echo "Do something"
      }
    }
  }
}
      
