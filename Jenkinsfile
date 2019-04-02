node {
    checkout scm

    docker.withRegistry('https://registry-1.docker.io/v2/', 'docker-hub-cred') {

        def customImage = docker.build("steve/alpine-smarter:1.0")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
