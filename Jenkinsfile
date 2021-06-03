node {
    checkout scm

    docker.withRegistry('http://168.194.255.179:5010') {

        def customImage = docker.build("my-image:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
