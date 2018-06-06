pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
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