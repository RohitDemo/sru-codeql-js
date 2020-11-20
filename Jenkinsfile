pipeline {
  agent any
  stages {
    stage('Download CodeQL') {
      steps {
        sh '''wget https://github.com/github/codeql-action/releases/download/codeql-bundle-20200826/codeql-runner-linux 
chmod +x codeql-runner-linux'''
      }
    }

    stage('run ls') {
      steps {
        sh 'ls -lah'
      }
    }

  }
}