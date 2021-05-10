pipeline {
  agent any
  stages {
    stage("testing"){
      steps {
            sh "docker info"
            sh "docker images"
            sh "kubectl version"
            sh "helm version"
      }
    }
  }
}
