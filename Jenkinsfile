pipeline {
  agent any
  stages {
    stage('Bulid') {
      steps {
        echo 'Bulid Complited'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test Stages') {
          steps {
            echo 'Running test 2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test 1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploymint Completet'
      }
    }

  }
}