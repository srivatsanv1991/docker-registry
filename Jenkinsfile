node {
    checkout scm

    docker.withRegistry('https://registry.example.com', 'credentials-id') {

        def customImage = docker.build("steve/alpine-smarter:1.0")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
