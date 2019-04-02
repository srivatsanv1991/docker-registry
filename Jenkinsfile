node {
    checkout scm

    docker.withRegistry('https://cloud.docker.com/u/srivatsanv1991/repository/docker/srivatsanv1991/srivatsanv', 'docker-hub-cred') {

        def customImage = docker.build("steve/alpine-smarter:1.0")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
