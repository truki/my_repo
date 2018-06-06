pipeline {
  agent any
  stages {
    stage('First stage') {
      parallel {
        stage('First stage - 1') {
          steps {
            echo 'Testing'
            sh 'echo "Hello BB"'
          }
        }
        stage('Pull repo') {
          steps {
            git(url: 'https://github.com/truki/ArasaacBot.git', branch: 'master')
          }
        }
      }
    }
  }
}
