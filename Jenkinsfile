pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'I want to plan my app development'
      }
    }

    stage('code') {
      steps {
        echo 'dev team start coding '
      }
    }

    stage('build') {
      steps {
        echo 'build the app'
      }
    }

    stage('test ') {
      parallel {
        stage('test ') {
          steps {
            echo 'testing team perform testing'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy war files'
          }
        }

        stage('release') {
          steps {
            echo 'move build to release'
          }
        }

        stage('operate ') {
          steps {
            echo 'test the app functionality'
          }
        }

      }
    }

  }
}