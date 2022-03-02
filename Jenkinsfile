
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
        sh '''
        docker cp /root/workspace/Montserrat/Monche/target/sparkjava-hello-world-1.0.war tomcat://usr/local/tomcat/webapps
        '''
      }
    }
  }
}
      
