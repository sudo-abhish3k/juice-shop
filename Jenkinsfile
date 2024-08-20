node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
     bat "C:/Users/Admin/Downloads/sonar-scanner-cli-6.0.0.4432-windows/sonar-scanner-6.0.0.4432-windows/bin/sonar-scanner.bat -X"
    }
  }
