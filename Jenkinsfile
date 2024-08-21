node {
  stage('SCM') {
    checkout scm
  }
  stage('SCA via Snyk') {
           steps {
               script {
                       withCredentials([string(credentialsId: 'bf9c4c75-1679-4a71-a2ec-37b243fd2b87', variable: 'SNYK_TOKEN')]) {
                       bat 'snyk monitor --token=$SNYK_TOKEN'
                   }
               }
           }
       }
}
