pipeline {
  agent {
    node {
      label 'ubuntu-2004-gce'
    }

  }
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'hello from blue ocean'
        sh 'echo \'hello from blue ocean\''
      }
    }

    stage('na') {
      steps {
        input(message: 'Deploy to stage?', ok: 'OK', submitter: 'miguelmont')
      }
    }

  }
}