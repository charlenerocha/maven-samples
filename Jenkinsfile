pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/charlenerocha/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}