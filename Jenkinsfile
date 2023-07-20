pipeline {
  agent any
  stages {
    stage('init env') {
      steps {
        echo 'it\'s mount driver'
        bat(script: 'net use X: \\\\172.16.161.111\\cimaster welcome /user:cimaster /persistent:yes', returnStatus: true, returnStdout: true)
        bat(script: 'dir', returnStatus: true, returnStdout: true)
      }
    }

    stage('mount driver to local') {
      steps {
        echo 'mount drivers'
        bat(script: 'dir', returnStatus: true, returnStdout: true)
      }
    }

  }
}