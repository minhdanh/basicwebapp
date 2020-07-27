pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "Hello world"'
        echo 'Hello world'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Test passed'
          }
        }

        stage('intergration tests') {
          steps {
            echo 'Tests passed'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployed'
      }
    }

  }
}