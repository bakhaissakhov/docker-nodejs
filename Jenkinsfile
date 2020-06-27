node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'dockerhub-bakha') {

        def customImage = docker.build("bakhaissakhov/nodejs}")  

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
