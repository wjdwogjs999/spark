pipeline {
  agent any
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

        stage('stage3') {
          steps {
            sh 'echo "stage2"'
            mail(subject: 'asdasd', body: 'asdasdasd')
          }
        }

      }
    }

    stage('error') {
      parallel {
        stage('error') {
          steps {
            echo 'error'
            retry(count: 2) {
              sh 'echo "hello"'
            }

          }
        }

        stage('success') {
          agent any
          steps {
            echo 'success'
            git 'dasdsadas'
          }
        }

        stage('czxczxcx') {
          steps {
            timeout(time: 23)
          }
        }

      }
    }

    stage('one') {
      steps {
        sh 'ecdcfafdasf'
      }
    }

  }
  environment {
    bodoru = 'value'
  }
}