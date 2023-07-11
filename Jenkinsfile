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
    stage(sample){
        steps{
          sh 'echo hii'
        }
    }
      }
}
