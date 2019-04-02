node {
checkout scm
 def customImage = docker.build “srivatsan/alpine-smarter:$BUILD_NUMBER”

    docker.withRegistry('', 'docker-hub-cred') {

        customImage.push()
    }
}
