node{
stage('docker build/push') {
docker.withDockerRegistry('https://hub.docker.com/','docker-hub-cred')
                    def app=docker.build("srivatsanv1991/srivatsanv:${commit_id}", '.').push()
}
}
