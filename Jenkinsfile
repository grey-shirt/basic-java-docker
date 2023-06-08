def imageName = 'grey-shirt/basic-java-docker'

node('workers'){
    stage('Checkout'){
        checkout scm
        }

    stage('Build Image'){
        def imageTest= docker.build("${imageName}",
        "-f Dockerfile .")
    }
}