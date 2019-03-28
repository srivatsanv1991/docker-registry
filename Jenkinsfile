pipeline{
    environment {
        registry = "docker_hub_account/repository_name"
        registryCredential = "dockerhub"
    }


    stages{
        stage('Building Image'){
            steps{
                script{
                    docker.build.registry+":$BUILD_NUMBER"
                }
            }
        }
    }
}


