pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Say Hello') {
      steps {
        echo "Hello Sriram! Jenkins is working "
      }
    }
  }
}
