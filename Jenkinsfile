pipeline {
  agent any
  stages {
    stage('newSparkStage1') {
      steps {
        sh 'echo "newSpark"'
        echo 'hello'
      }
    }

    stage('error') {
      steps {
        build 'test'
      }
    }

  }
}