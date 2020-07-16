pipeline {
  agent none
  stages {
    stage('newSparkStage1') {
      parallel {
        stage('newSparkStage1') {
          steps {
            sh 'echo "newSpark"'
            echo 'hello'
          }
        }

        stage('stage2') {
          steps {
            echo 'hi'
          }
        }

      }
    }

    stage('error') {
      parallel {
        stage('error') {
          steps {
            echo 'error'
          }
        }

        stage('success') {
          steps {
            echo 'success'
          }
        }

      }
    }

  }
  environment {
    bodoru = 'value'
  }
}