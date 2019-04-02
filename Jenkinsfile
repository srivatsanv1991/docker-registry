node {
    checkout scm

    docker.withRegistry('https://index.docker.io/v1/', 'docker-hub-cred') {

        def customImage = docker.build("steve/alpine-smarter:1.0")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
