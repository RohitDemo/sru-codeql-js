pipeline {
  agent any
  stages {
    stage('CodeQL') {
      steps {
        sh '''ls -lah
wget https://github.com/github/codeql-action/releases/download/codeql-bundle-20200826/codeql-runner-linux 
chmod +x codeql-runner-linux
ls -lah
codeql-runner-linux init --repository rohitdemo/sru-codeql-js --github-url https://github.com --github-auth 615a834ba92b489dbeb156fd37ea347bc94e97c4
codeql-runner-linux analyze --repository rohitdemo/sru-codeql-js --github-url https://github.com --github-auth 615a834ba92b489dbeb156fd37ea347bc94e97c4'''
      }
    }

  }
}