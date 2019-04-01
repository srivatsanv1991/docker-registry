node{
stage('docker build/push') {
  docker.withDockerRegistry('https://index.docker.io/','docker-hub-cred'){
                    def app=docker.build("srivatsanv1991/srivatsanv:${commit_id}", '.')
    app.push()
  }
}
}
