node{
stage('docker build/push') {
  docker.withDockerRegistry('https://index.docker.io/','docker-hub-cred'){
                    def app=docker.build("srivatsanv1991/steve/alpine-smarter:1.0", '.')
    app.push()
  }
}
}
