pipeline {
  agent any
  stages {
    stage('Helloworld') {
      steps {
        sh 'echo -e "This is my first Pipeline :Hello"'
      }
    }

    stage('Stage2') {
      steps {
        git(url: 'https://github.com/jayesh271184/dhtechlab.git', branch: 'shell', changelog: true)
      }
    }

    stage('RunScript') {
      steps {
        sh 'sh FileCount.sh'
      }
    }

  }
}