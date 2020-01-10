pipeline {
  agent any
  stages {
    stage('') {
      steps {
        echo 'Build Stage'
        sh '''/usr/local/src/apache-maven/bin/mvn clean verify -DskipITs=true
'''
        junit '**/target/surefire-reports/TEST-*.xml'
        archiveArtifacts 'target/*.jar'
      }
    }

  }
}