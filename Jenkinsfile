pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/mitesh51/AntExample.git', branch: 'master', poll: true)
      }
    }
    stage('Build') {
      steps {
        tool 'apache-ant-1.10.5'
      }
    }
  }
}