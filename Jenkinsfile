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
      steps {
        build 'test'
      }
    }

  }
}