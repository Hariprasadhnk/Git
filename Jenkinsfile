pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Code under stage'
          }
        }

        stage('code') {
          steps {
            echo 'code depoly'
          }
        }

      }
    }

    stage('QA') {
      steps {
        echo 'Test Code'
      }
    }

    stage('Prod') {
      steps {
        echo 'deploy'
      }
    }

  }
}