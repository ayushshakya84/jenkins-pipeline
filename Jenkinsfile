pipeline {
  agent {
    node {
      label 'rhel-cli-node'
    }

  }
  stages {
    stage('scm') {
      parallel {
        stage('scm') {
          steps {
            git 'https://github.com/ayushshakya84/jenkins-pipeline.git'
            git(url: 'https://github.com/ayushshakya84/jenkins-pipeline.git', branch: 'master')
          }
        }

        stage('') {
          steps {
            sleep 2
          }
        }

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