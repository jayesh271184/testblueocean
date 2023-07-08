pipeline {
  agent any
  stages {
    stage('Helloworld') {
      parallel {
        stage('Helloworld') {
          steps {
            sh 'echo -e "This is my first Pipeline :Hello"'
          }
        }

        stage('Stage7') {
          steps {
            git(url: 'https://github.com/jayesh271184/dhtechlab.git', branch: 'main', changelog: true)
          }
        }

      }
    }

    stage('Stage2') {
      parallel {
        stage('Stage2') {
          steps {
            git(url: 'https://github.com/jayesh271184/dhtechlab.git', branch: 'shell', changelog: true)
          }
        }

        stage('PrintName') {
          steps {
            echo 'This is created by jayesh Shah'
          }
        }

      }
    }

    stage('RunScript') {
      parallel {
        stage('RunScript') {
          steps {
            sh 'sh FileCount.sh'
          }
        }

        stage('error') {
          steps {
            sh '''pwd


'''
          }
        }

      }
    }

  }
}