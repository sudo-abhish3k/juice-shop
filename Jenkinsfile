node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    bat 'C:/Users/Admin/Downloads/sonar-scanner-cli-5.0.1.3006-windows/sonar-scanner-5.0.1.3006-windows/bin/sonar-scanner.bat -D"sonar.login=%SONAR_TOKEN%" -X'
  }
}
