node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'Dockerid') {

        def customImage = docker.build("sysadminbioenable/nodejsapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
