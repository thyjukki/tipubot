pipeline {
  agent {
    label "linux"
  }
  stages {
    stage("SonarQube Analysis") {
      steps {
        withSonarQubeEnv('SonarQube Jukki') {
          sh "${tool 'Sonarscanner_latest'}/bin/sonar-scanner"
        }
      }
    }
  }
}