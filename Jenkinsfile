pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn install'
      }
    }

    stage('artifact') {
      steps {
        archiveArtifacts '**/*.war'
      }
    }

  }
  environment {
    person = 'subhash'
  }
}