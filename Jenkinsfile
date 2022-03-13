pipeline {
  agent any
  tools {
     maven 'M2_HOME'
  }
  stages {
    stage ( 'build'){
      steps {
        sh 'mvn clean'
        sh 'mvn install'
        sh 'mvn package'
      }
    }
    stage ( 'tset'){
      steps {
        echo "test step"
        sh 'mvn test'
      }
    }
    stage ( 'Deploy'){
      steps {
        echo "Deploy step"
        sleep 10
      }
    }
    stage ( 'Docker'){
      steps {
        echo "docker step"
        sleep 10
      }
    }
  }
}
 
