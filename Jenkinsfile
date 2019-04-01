node{
  checkout scm
  docker.withDockerRegistry('https://index.docker.io/','docker-hub-cred'){
                    def app=docker.build("steve/alpine-smarter:1.0", '.')
    app.push()
  }
}
