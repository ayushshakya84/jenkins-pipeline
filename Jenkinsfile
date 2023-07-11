pipeline {
  agent {
    node {
      label 'rhel-cli-node'
    }

  }
  stages {
    stage('scm') {
      steps {
        git 'https://github.com/ayushshakya84/jenkins-pipeline.git'
      }
    }

    stage('testing') {
      steps {
        echo 'testing successfully'
      }
    }

    stage('deploying') {
      steps {
        sh 'sudo cp index.html /var/www/html'
      }
    }

  }
}