node {

    checkout scm

    docker.withRegistry('https://hub.docker.com/', 'dockerHub') {

        def customImage = docker.build("node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
