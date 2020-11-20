pipeline {
  agent any
  stages {
    stage('CodeQL') {
      steps {
        sh '''ls -lah
wget https://github.com/github/codeql-action/releases/download/codeql-bundle-20200826/codeql-runner-linux 
chmod +x codeql-runner-linux
ls -lah
./codeql-runner-linux init --repository rohitdemo/sru-codeql-js --github-url https://github.com --github-auth 1555914c55939fa544f3a83eadc1e3161a829da3
./codeql-runner-linux analyze --repository rohitdemo/sru-codeql-js --github-url https://github.com --github-auth 1555914c55939fa544f3a83eadc1e3161a829da3'''
      }
    }

  }
}