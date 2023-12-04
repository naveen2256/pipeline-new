pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is devlopment'
      }
    }

    stage('build') {
      steps {
        echo 'this is build state'
      }
    }

    stage('test') {
      steps {
        echo 'this is test state'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAT') {
          steps {
            echo 'this is uat state'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deploy state'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate state'
          }
        }

      }
    }

  }
}