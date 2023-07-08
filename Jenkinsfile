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
        git(url: 'https://github.com/jayesh271184/dhtechlab.git', branch: 'main')
      }
    }

  }
}