pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing'
          }
        }

        stage('parallel') {
          steps {
            echo 'building'
          }
        }

      }
    }

    stage('build') {
      steps {
        echo 'building'
      }
    }

    stage('clean up') {
      steps {
        echo 'cleaning'
      }
    }

  }
}