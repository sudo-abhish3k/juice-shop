node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
  withCredentials([string(credentialsId: 'sonarqube', variable: 'envsonar')]) {
    bat 'C:/Users/Admin/Downloads/sonar-scanner-cli-6.1.0.4477-windows-x64/sonar-scanner-6.1.0.4477-windows-x64/bin/sonar-scanner.bat -D"sonar.login=admin -D"sonar.password=%envsonar%" D"sonar.host.url=http://localhost:9000" -X'
  }
}
