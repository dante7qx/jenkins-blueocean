pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }
        stage('ie') {
          steps {
            echo 'ie test'
          }
        }
        stage('firefox') {
          steps {
            echo 'firefox test'
          }
        }
      }
    }
    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 2
      }
    }
  }
}