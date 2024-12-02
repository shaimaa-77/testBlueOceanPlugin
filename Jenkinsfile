pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('test stages') {
      parallel {
        stage('Test2') {
          steps {
            echo 'Test compeleted'
          }
        }

        stage('Test1') {
          steps {
            echo 'running test 1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy compeleted'
      }
    }

  }
}