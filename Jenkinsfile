pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Clean the ws'
        sh 'this is clean project'
      }
    }

    stage('Build2') {
      parallel {
        stage('Build2') {
          steps {
            build 'Freestyle'
          }
        }

        stage('build3') {
          steps {
            echo 'hello'
          }
        }

      }
    }

    stage('Ending') {
      steps {
        mail(subject: 'mail@gmail.com', body: 'mail', from: 'vaibhavi', replyTo: 'vaibhavi', to: 'vaibhavi')
      }
    }

  }
}