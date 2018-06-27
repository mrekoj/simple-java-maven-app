pipeline {
  agent {
    docker {
      args 'args \'-v /root/.m2:/root/.m2\''
      image 'image \'maven:3-alpine\''
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'sh \'mvn -B -DskipTests clean package\''
      }
    }
  }
}