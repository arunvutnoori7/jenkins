pipeline {
  agent any
  stages {
    stage('check code') {
      steps {
        git(url: 'https://github.com/arunvutnoori7/jenkins', branch: 'main')
      }
    }

    stage('npm') {
      steps {
        sh 'npm i --force'
      }
    }

    stage('build') {
      steps {
        sh 'npm start'
      }
    }

  }
}