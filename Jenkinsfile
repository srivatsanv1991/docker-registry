node {
    checkout scm
def customImage = docker.build("steve/alpine-smarter:1.0")
  
    docker.withRegistry('https://index.docker.io/v1/', 'docker-hub-cred') {

        

        /* Push the container to the custom Registry */
        customImage.push('latest')
    }
}
