pipeline {
  agent {label 'lnx2'}
  tools {
    jdk 'jdk8'
    maven 'maven3'
  }
  stages {
    stage('test java installation') {
      steps {
        sh 'echo $HOSTNAME'
        sh 'java -version'
        sh 'which java'
      }
   }
    stage('test maven installation') {
      steps {
        sh 'echo $HOSTNAME'
        sh 'mvn -version'
        sh 'which mvn'
      }
    }
    stage('test ansible installation') {
      steps {
        sh 'echo $HOSTNAME'
        sh 'ansible --version'
        sh 'which ansible'
      }
    }
  }
}
