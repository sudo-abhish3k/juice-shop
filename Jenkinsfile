node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    bat 'C:/Users/Admin/Downloads/sonar-scanner-cli-6.1.0.4477-windows-x64/sonar-scanner-6.1.0.4477-windows-x64/bin/sonar-scanner.bat -D"sonar.host.url=http://localhost:9000" -D"sonar.login=admin" -D"sonar.password=Paladion123$" -X'
  }
}
