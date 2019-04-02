node {
    checkout scm
    def customImage = docker.build "srivatsanv1991/srivatsanv:$BUILD_NUMBER"
  
    docker.withRegistry('', 'docker-hub-cred') {
        customImage.push()
    }
}
