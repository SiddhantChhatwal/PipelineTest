pipeline {
  agent any
  tools { 
      maven 'MAVEN_HOME' 
      jdk 'JAVA_HOME'
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        sh 'mvn deploy'
      }
    }
  }
}
