pipeline {
  agent any
  tools{
    maven 'M2_HOME'
  }
  stages {
    stage('build'){
      steps {
       sh 'mvn clean'
       sh 'mvn install'
       sh 'mvn package'    
      }
    }
     stage('test'){
      steps {
        echo "test step"
        sh 'mvn test'
      }
    }
     stage('work'){
      steps {
        echo "work steps"
        sleep 10
      }
    }
     stage('Deploy'){
      steps {
        echo "build steps"
        sleep 10
      }
    }
  }   
}    
