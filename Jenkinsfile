pipeline {
  agent any
  stages {
    stage('Bulid') {
      steps {
        echo 'Welcome to Bulid Level'
      }
    }

    stage('Stages') {
      parallel {
        stage('Stages') {
          steps {
            echo 'Print test 1'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Print Test 2'
          }
        }

      }
    }

    stage('Deploy Stage') {
      steps {
        input(message: 'Are You Sure to Deply', ok: 'Yes Im ready')
        echo 'Wlecome to Deploy stage'
      }
    }

  }
}