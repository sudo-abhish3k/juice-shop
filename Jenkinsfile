node {
  stage('SCM') {
    checkout scm
  }
  
  stage('SCA via Snyk') {
    script {
      bat "snyk monitor --token=bf9c4c75-1679-4a71-a2ec-37b243fd2b87"
    }
  }
}
