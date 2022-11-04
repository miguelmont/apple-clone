pipeline {
  agent {
    docker {
      image 'jenkins/ssh-agent:alpine'
      args '-u root -v /var/bin/jenkins'
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
        archiveArtifacts(fingerprint: true, artifacts: '*')
      }
    }

  }
}