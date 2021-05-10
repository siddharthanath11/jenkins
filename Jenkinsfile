pipeline {
  agent any
  stages {
    stage('Checkout') {
        steps {
            git(
                branch: 'master',
                credentialsId: 'JENKINS_GLOBAL_CREDENTIAL_ID',
                url: 'https://github.com/test/test'
            )
            script {
                sh 'git checkout master'
            }
        }
    }
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
