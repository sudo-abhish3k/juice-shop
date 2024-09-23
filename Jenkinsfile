<<<<<<< HEAD
node {
    stage('SCM') {
        checkout scm
    }

    stage('Secret Scanning Trufflehog') {
        bat 'docker run trufflesecurity/trufflehog:latest git https://github.com/sudo-abhish3k/juice-shop --only-verified --json'
    }
  
    stage('SCA via Snyk') {
        script {
           bat "C:/Users/Admin/AppData/Roaming/npm/snyk monitor --token=bf9c4c75-1679-4a71-a2ec-37b243fd2b87"
        }
    }
  
    stage('SonarQube Analysis') {
        withCredentials([string(credentialsId: 'sonarqube', variable: 'envsonar')]) {
            bat 'C:/Users/Admin/Downloads/sonar-scanner-cli-6.1.0.4477-windows-x64/sonar-scanner-6.1.0.4477-windows-x64/bin/sonar-scanner.bat -Dsonar.token=%envsonar% -Dsonar.host.url=http://localhost:9000 -X'
        }
    }
}
=======
node {
    stage('SCM') {
        checkout scm
    }

    stage('SCA via Snyk') {
        script {
           bat "C:/Users/Admin/AppData/Roaming/npm/snyk monitor --token=bf9c4c75-1679-4a71-a2ec-37b243fd2b87"
        }
    }
  
    stage('SonarQube Analysis') {
        withCredentials([string(credentialsId: 'sonarqube', variable: 'envsonar')]) {
            bat 'C:/Users/Admin/Downloads/sonar-scanner-cli-6.1.0.4477-windows-x64/sonar-scanner-6.1.0.4477-windows-x64/bin/sonar-scanner.bat -Dsonar.token=%envsonar% -Dsonar.host.url=http://localhost:9000 -X'
        }
    }
}
>>>>>>> 58dad5f8bd39801b07aebfd5153b7dc9e717cdd2
